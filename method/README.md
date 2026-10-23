# How the signs were read and measured

This folder explains how the readings in `../data/` were made, and how far they can be trusted. The full working code is not published here: it depends on our own tools and language resources. What is here is enough to see what was done, to recompute the measured numbers on the known text, and to reproduce the decode exactly (`../decode/`).

## The cipher

Matignon's Cipher-3, as reconstructed by Satoshi Tomokiyo (<https://cryptiana.web.fc2.com/code/henryiii.htm>): a substitution of about fifty signs (letters, digits and invented shapes), with homophones, a few signs for groups of letters or short words, and a few code signs. The two y-shaped signs stand for t or n, and an 8-shaped sign for v or o. There are no word divisions in the cipher.

## Step 1: a letter with a known answer

BnF fr. 15572 ff. 277r–278r is a letter in the same cipher and the same spaced hand; its decipherment made at the time is on ff. 279r–280r. Claude read ff. 279r and 280r from the image ([../data/known-text/](../data/known-text/)). f. 279v was not read. No modern reading of these leaves was used.

## Step 2: the reference sheet and the key check

The signs of f. 277r were cut out by code (deskew, line tracking, connected components), grouped by shape (k-means), and the groups named by Claude from the images. The reference sheet [sheet-v2.png](sheet-v2.png) has 50 visual names with 2–5 examples each, all cut from f. 277r ([sheet-v2.json](sheet-v2.json) lists the names and the example indices). The names are labels for shapes only; the reader is never told the values.

A first reader pass over f. 277r (and f. 278r) was aligned by code with the decipherment (soft EM alignment, units of up to 8 letters). The values it gives ([../data/known-text/em-key-v2.json](../data/known-text/em-key-v2.json)) agree with Tomokiyo's published table on every frequent sign compared. On the f. 277r re-read, two reader calls ended in a refusal; those lines (28–32) were left out of the alignment.

## Step 3: Claude reads the signs

Each manuscript line was straightened and cut into pieces. The pieces were shown to Claude (model `claude-opus-5-5`, effort low, 12 pieces per call) under the reference sheet, with the instruction to name every sign from left to right. The answers were treated as data only and parsed into sign names. Three passes were made with different cuts and magnifications (see `passes` in `../data/<page>/reading.json`).

## Step 4: the vote

The three readings of a line are aligned by edit distance, and the majority name is taken at each place (ties: pass a). A sign seen by only one pass is dropped unless pass a has it. Every position keeps the names given, most voted first (`../data/<page>/reading.json`).

## Step 5: corrections, only where the image supports them

Code proposed, for each page, the 10 positions where another pass's name lowers the word-decode cost of the line most. Each proposal was looked at on the straightened line image and applied only when the image shows the proposed sign. 60 were looked at, 25 applied (`../data/<page>/corrections.json`). The recurrent case was an 8-shaped o-sign that the readers had named g. The proposals for f. 381v were void after that page was re-cut (its last line had first fallen outside the text box), so none was applied there.

## Step 6: from signs to letters

The key ([../data/key-cipher3.json](../data/key-cipher3.json)) is applied to the signs. For the two-valued signs, a word-level decoder (a dynamic programme over the signs with a period French dictionary) chose one of the listed values at each place; it can only choose among the listed values. Every choice is written in `../data/<page>/key.json` under `choices`, so the decode itself is mechanical and anyone can repeat it with [../decode/decode.py](../decode/decode.py).

## Step 7: word breaks (Normalised text)

The Normalised text in `../reading/ff379-381-french.md` adds word breaks by the same word decoder. A stretch that matches no dictionary word is shown in [brackets]. No letter is changed, added or removed; the letters of Normalised equal the letters of Literal on every line.

## Measurement on known text

Held-out lines 12–18 of fr. 15572 f. 278r (238 signs) were read sign by sign from the image by Claude as a reference ([../data/known-text/ref-278r-l12-18.txt](../data/known-text/ref-278r-l12-18.txt)); where the image does not decide, two names are accepted. The reference was checked by decoding it against the decipherment on f. 280r. Sign accuracy = reference signs read right / reference signs, after an edit-distance alignment per line. [score_heldout.py](score_heldout.py) recomputes it (Python 3, standard library):

```
$ python3 method/score_heldout.py
pass_a  227 / 238 reference signs read right -> sign accuracy 0.9538
pass_b  225 / 238 reference signs read right -> sign accuracy 0.9454
pass_c  220 / 238 reference signs read right -> sign accuracy 0.9244
vote    229 / 238 reference signs read right -> sign accuracy 0.9622
```

Strict scoring (first accepted name only) gives 0.9328 for the vote (`--strict`).

Cautions: the reference was made by Claude, the same model as the reader, after pass a had been seen; its independence is the decode check against the 1586 decipherment, not a second reader. At plaintext level the voted reading, decoded with the key, matches the f. 280r text on 0.69 of letters; the shortfall is mostly not the reader (code signs the key does not know, the n/t choice, text the decipherer wrote out where the cipher abbreviates, and our own reading of the cursive decipherment). That figure is a floor.

## Controls

A decoder with a dictionary makes almost anything look a little like its language. So each page was also decoded with its signs shuffled into random order (seeds 1, 2, 3), with the same key and decoder. The reading sits at 3.874–4.42 bits per letter, the shuffled controls at 5.784–6.358; dictionary cover 0.8607–0.8964 against 0.6742–0.78. The last fifth of each page decoded on its own reads like the rest. The calibration page f. 278r (lines 10–26, voted), read and decoded the same way, gives 3.54 bits per letter and 0.92 cover (optimistic: the key values were aligned partly on that page); its decipherment text itself scores 2.65. Numbers per page: `../data/<page>/controls.json`.

## What this does not show

- It is a machine reading, voted; it awaits a palaeographer's reading.
- The error rate on these pages is probably higher than on the calibration lines (the passes agree less often).
- Several code signs are unidentified, and the n/t choice is made by a dictionary decoder.

## Images

`sheet-v2.png`: crops of BnF, Français 15572, f. 277r, from Gallica (ark:/12148/btv1b9061879d, view 286). Source gallica.bnf.fr / Bibliothèque nationale de France. Free non-commercial reuse with this source line; commercial reuse needs the BnF's permission. Not under this repository's CC BY licence.
