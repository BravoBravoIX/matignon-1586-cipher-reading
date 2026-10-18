# The Matignon cipher despatch of autumn 1586: a first reading of the whole despatch

**BnF, Français 15573, ff. 379r–381v.** A despatch of autumn 1586 written wholly in cipher, six pages, addressed to King Henri III and probably sent by Marshal Jacques de Matignon from Guyenne. It uses the cipher that Satoshi Tomokiyo calls **Matignon's Cipher-3**.

> **First reading of the whole despatch, version 0.4 (19 October 2026): work in progress, partial in places.** Every page is read; the remaining gaps are listed with their causes. Versions 0.1-0.3 were published on 18 October 2026.
>
> **Satoshi Tomokiyo published the opening line earlier**, on his page of Henri III's ciphers, which lists this letter as undeciphered and gives Matignon's Cipher-3: <https://cryptiana.web.fc2.com/code/henryiii.htm>. His opening reads "a ce quil plaist [votre] majeste me commander lui donner advis pour lentre de [votre] arme…". **Our reading of the opening matches it** (*a ce [q]uil … maieste*), and it was made without using his text.
>
> Beyond that line, as far as our search found (see [PRIOR-ART.md](PRIOR-ART.md)), no reading of these pages has been published. Updates will follow.

## What changed since version 0.1

- **0.2:** five reader passes voted per sign (0.1 had three); the decoder works on a whole page and chooses the letter of each two-valued sign by whole French words.
- **0.3:** sign shapes the reference sheet had merged were split on the image, following Tomokiyo's table (each change needed two agreeing reader answers and a look at the crop); key values added only from aligned occurrences in the 1586 decipherments (fr. 15572 ff. 279-280) or Tomokiyo's table, doubtful values flagged; four correction rounds decided on the image (34 changes kept, 72 proposed changes rejected); 164 period place names, persons and words added to the lexicon, each tagged by source (`data/lexicon-additions.tsv`).
- **0.4:** six key values learnt from a further Cipher-3 letter deciphered at the time, fr. 15570 ff. 271r-272r (September 1585, decipherment on f. 273): a long zigzag = ss, a 9 in a circle = *par*, d = *vostre* (confirmed: "vostre maieste" five times), and, each from one occurrence and flagged doubtful, a barred double o = the code group *le roy de Navarre*, "13" = *faict*, a figure 6 = s. The old key already read that 1585 letter as French before any change, an independent check of the key. Every sign whose class changed was sorted by eye and confirmed by two agreeing reader answers; one more image-decided correction round.

Share of signs that fall inside French words, per page. The known-answer page (fr. 15572 f. 278r, read and decoded the same way) scores 0.907 in v0.4, and the same signs shuffled score 0.59-0.70:

| page | v0.1 | v0.2 | v0.3 | v0.4 |
|---|---|---|---|---|
| f. 379r | 0.734 | 0.861 | 0.950 | 0.950 |
| f. 379v | 0.779 | 0.864 | 0.902 | 0.902 |
| f. 380r | 0.726 | 0.839 | 0.898 | 0.913 |
| f. 380v | 0.780 | 0.885 | 0.923 | 0.925 |
| f. 381r | 0.755 | 0.832 | 0.899 | 0.904 |
| f. 381v | 0.722 | 0.810 | 0.915 | 0.932 |

In v0.4, 119 items remain (`reading/unresolved-v0.4.md`): 104 explained (doubtful word 67, damage 25, code sign 8, reader doubt 4) and 15 runs of clear signs not yet read; five code signs are still unknown (they do not occur in the 1585 letter). The reading now names the King of Navarre, "your sister" at Agen, the artillery brought out of Navarrenx and "fifteen to sixteen thousand crowns". Next: further deciphered Cipher-3 letters for the five unknown signs.

## What the despatch is about

The readable stretches are a military report to the King on the Guyenne campaign of 1586: places on the Garonne, the Isle and the Dordogne; Castillon; the Mas de Verdun; the revenue the Huguenots draw from the river trade; the army's movements, artillery and regiments. The sender's name does not appear in the readable stretches; "probably Matignon" rests on the cipher (Tomokiyo's attribution) and the content. See [reading/ff379-381-english.md](reading/ff379-381-english.md) for an English gist, labelled as such.

## Status of each page

*Version 0.1 figures (three passes), kept for the record; the current per-page figures are in the table above.*

All pages were read the same way: three reader passes, voted, then image-checked corrections. 127 lines and 2834 signs in all.

| page | Gallica view | lines | signs | all three passes agree | corrections applied |
|---|---|---|---|---|---|
| f. 379r | 740 | 22 | 503 | 0.7913 | 3 |
| f. 379v | 741 | 23 | 490 | 0.8174 | 6 |
| f. 380r | 742 | 22 | 492 | 0.811 | 5 |
| f. 380v | 743 | 24 | 531 | 0.7665 | 5 |
| f. 381r | 744 | 23 | 523 | 0.8184 | 6 |
| f. 381v | 745 | 13 | 295 | 0.8034 | 0 |

## What is here

| folder | contents |
|---|---|
| [reading/](reading/) | The French text of each page (Literal = exactly what the key gives; Normalised = the same letters with word breaks made by code) and an English gist of the readable stretches |
| [data/](data/) | Per page: the signs as read (`signs.txt`, one manuscript line per row; `reading.json` with the votes for every sign), the key with the value chosen at every occurrence of a two-valued sign (`key.json`), the literal plaintext, corrections and controls. `key-cipher3.json` is the key with the origin of every value. `known-text/` holds the calibration material |
| [decode/](decode/) | `decode.py`, a short stand-alone script (Python 3 standard library) that applies `key.json` to `signs.txt`, and `check.sh`, which reproduces all six pages byte for byte |
| [method/](method/) | How the signs were read (the prompt given to Claude, the reference sheet of signs), the vote, the corrections, the key, the controls and the measurement on known text |
| [PRIOR-ART.md](PRIOR-ART.md) | The prior-art search: what was searched, where, and every query with its result count |
| [NUMBERS.md](NUMBERS.md) | Where every number in this README comes from |

## The pages and the images

The images are on Gallica, BnF Français 15573, ark:/12148/btv1b90618780 (Source gallica.bnf.fr / BnF):

- f. 379r, view 740: <https://gallica.bnf.fr/ark:/12148/btv1b90618780/f740.item>
- f. 379v, view 741: <https://gallica.bnf.fr/ark:/12148/btv1b90618780/f741.item>
- f. 380r, view 742: <https://gallica.bnf.fr/ark:/12148/btv1b90618780/f742.item>
- f. 380v, view 743: <https://gallica.bnf.fr/ark:/12148/btv1b90618780/f743.item>
- f. 381r, view 744: <https://gallica.bnf.fr/ark:/12148/btv1b90618780/f744.item>
- f. 381v, view 745: <https://gallica.bnf.fr/ark:/12148/btv1b90618780/f745.item>
- view 739 is the preceding leaf, f. 378, a separate letter in clear (from the inhabitants of Tarascon, per the BnF catalogue), not a covering letter.

The calibration letter, in the same cipher and the same hand, is BnF Français 15572, ark:/12148/btv1b9061879d:

- ff. 277r–278r, the cipher letter: views 286 (right page = f. 277r) and 288 (left = f. 277v, right = f. 278r): <https://gallica.bnf.fr/ark:/12148/btv1b9061879d/f286.item>, <https://gallica.bnf.fr/ark:/12148/btv1b9061879d/f288.item>
- ff. 279r–280r, its decipherment made at the time: views 289 (right page = f. 279r) and 290: <https://gallica.bnf.fr/ark:/12148/btv1b9061879d/f289.item>, <https://gallica.bnf.fr/ark:/12148/btv1b9061879d/f290.item>

The page images are not copied here. The reference sheet in `method/` is made of small crops of fr. 15572 f. 277r (see the image terms below).

## The key

The key is **Satoshi Tomokiyo's reconstruction** of Matignon's Cipher-3, published on his page of Henri III's ciphers (<https://cryptiana.web.fc2.com/code/henryiii.htm>). We do not reproduce his key image; please see it on his page. We checked its values against the 1586 decipherment of the sister letter: our reading of fr. 15572 ff. 277r and 278r was aligned by code with their contemporary decipherment on ff. 279r and 280r, and the values that alignment gives agree with Tomokiyo's table on every frequent sign compared. A few values that his table does not give were taken from that alignment, and are marked so. Every value in [data/key-cipher3.json](data/key-cipher3.json) carries its origin: `T` (Tomokiyo's table), `E` (the alignment with the 1586 decipherment), `T+E` (both), `E?` (the alignment, few occurrences: doubtful).

- Most signs stand for one letter; several signs share a letter (homophones).
- Some signs stand for a group of letters or a short word: for example *de*, *la*, *le*, *que*, *qui*, *pour*, *et*, and a doubled *ll*.
- Three signs stand for two letters: the two y-shaped signs (`y`, `yv`) for **t or n**, and the 8-shaped sign for **v or o**. For these, a word-level decoder with a period French dictionary chose one value at each place, and every choice is written in `data/<page>/key.json`.
- Some code signs are not identified (`x`, `oo`, `#`, `tri`, `excl`, `Lx2`, and a sign before *majesté*, probably *vostre*). They print as `·` (or `[?name]`).

## The method in plain words

*This describes version 0.1; later versions add the steps listed above.*

1. **A letter with a known answer.** fr. 15572 ff. 277r–278r is in the same cipher and hand, and its decipherment made at the time survives (ff. 279r–280r). We read that decipherment by eye.
2. **A reference sheet.** From f. 277r we cut a sheet of 50 sign shapes, 2–5 examples each, named by their look only (the names say nothing about meaning).
3. **Claude reads the signs.** Each line was cut into pieces, and the pieces were shown to Claude (Anthropic, model Opus 5.5) under the reference sheet, with the instruction to name every sign from left to right. This was done three times with different cuts and magnifications.
4. **Vote.** The three readings of each line were aligned and the majority name taken at each place.
5. **Corrections, only where the image supports them.** Code pointed out the 10 places per page where another pass's name would most improve the decode; each was looked at in the image and applied only if the image shows that sign. 25 were applied.
6. **Key applied mechanically.** The key turns each sign into its value; for the three two-valued signs the choice made by the word decoder is recorded. From then on the decode is a lookup that anyone can repeat with `decode/decode.py`.
7. **Word breaks by code** from a period French dictionary, for the Normalised text only. No letter is changed.
8. **Controls.** Every page was also decoded with its signs shuffled into a random order, in exactly the same way. The last fifth of each page was also decoded on its own.

Details are in [method/README.md](method/README.md).

## Measured numbers

*Calibration measurements on the known-answer letter (unchanged since version 0.1) and the version 0.1 controls; current per-page figures are in the table above.*

**Reader calibrated on known text.** The reader was measured on fr. 15572 f. 278r, lines 12–18 (238 signs), against their contemporary decipherment on ff. 279–280. Nothing in the sheet or the key was tuned on these lines. The reference signs were read by eye and checked by decoding against the decipherment on f. 280r.

| reader | sign accuracy (either name accepted where the eye cannot choose) |
|---|---|
| pass a / b / c | 0.9538 / 0.9454 / 0.9244 |
| **vote of the three passes** | **0.962** (0.933 strict, counting only the first accepted name) |

So the vote reads about **0.962 per sign (0.933 strict)** on known text: roughly one sign in twenty to thirty is wrong. On the target pages the three passes agree less often (0.7665–0.8184 of positions, against 0.87 on the calibration page), so the error rate there is probably higher than on the calibration page.

**Controls** (bits per letter under a period French 5-gram model, lower = more like French; dictionary cover = share of letters inside dictionary words of the word decode):

| page | signs | bits/letter, reading | bits/letter, shuffled seeds 1 / 2 / 3 | dict cover, reading | dict cover, shuffled 1 / 2 / 3 | held-out last fifth (bits / cover) |
|---|---|---|---|---|---|---|
| f. 379r | 503 | 4.42 | 6.236 / 6.323 / 6.257 | 0.8607 | 0.6832 / 0.6908 / 0.708 | 4.766 / 0.8571 |
| f. 379v | 490 | 3.874 | 6.024 / 6.358 / 6.261 | 0.8864 | 0.7121 / 0.7045 / 0.6742 | 3.359 / 0.9405 |
| f. 380r | 492 | 4.024 | 6.093 / 5.912 / 5.797 | 0.8863 | 0.7216 / 0.7294 / 0.7235 | 3.522 / 0.9341 |
| f. 380v | 531 | 4.088 | 5.915 / 5.796 / 5.958 | 0.8741 | 0.6976 / 0.7308 / 0.7255 | 4.321 / 0.8557 |
| f. 381r | 523 | 4.04 | 5.823 / 5.784 / 6.096 | 0.8964 | 0.78 / 0.7545 / 0.7127 | 3.698 / 0.8438 |
| f. 381v | 295 | 4.071 | 6.236 / 5.943 / 6.029 | 0.8677 | 0.6806 / 0.7419 / 0.7129 | 4.838 / 0.8085 |

The readings sit at 3.874–4.42 bits per letter with dictionary cover 0.8607–0.8964; the shuffled controls at 5.784–6.358 and 0.6742–0.78. The last fifth of each page, decoded on its own, reads like the rest. For comparison, the decipherment text of the calibration letter itself scores 2.65 bits per letter: the target pages read as French, but with many gaps.

## What is unresolved

*For the current list see `reading/unresolved-v0.4.md`; the text below describes version 0.1.*

- **Misread signs.** About one sign in twenty to thirty on known text, probably more on these pages. Stretches that match no dictionary word are shown in [brackets] in the Normalised text.
- **Code signs not identified**: `x`, `oo`, `#`, `tri`, `excl`, `Lx2`, and the sign before *majesté* (probably *vostre*, an inference only). They print as `·`.
- **The n/t choice** for the y-shaped signs is the main source of doubtful words; the 8-shaped sign (v/o) is a smaller one.
- **No palaeographer has checked it.** The English gist is Claude's, from our Normalised French; it is not literal plaintext.
- Line numbers of f. 381v run from 0 in `data/f381v/` (as in our working records) and from 1 in `reading/ff379-381-french.md`.

This is version 0.4. **Updates will follow** as more of the code signs are identified (from other letters in the same cipher) and the weakest stretches are read again.

## Prior art

Searched on 18 October 2026, and repeated the same day before this write-up (10:20–10:28 UTC): GitHub (code, repositories, issues, recent commits and pull requests of the active cipher-reading repositories), Tomokiyo's blog and pages, the web, the Bourdeau catalogue, Cryptoole and the Monaco Palace archives (fonds Matignon). **No reading of ff. 379r–381v was found** beyond Tomokiyo's opening line. One lead is unscreened: the Monaco Palace archives, series J 41 (Matignon's letters and minutes, 1562–1596), which might hold a minute of this despatch in clear. Every query and its result count is in [PRIOR-ART.md](PRIOR-ART.md).

## How to reproduce the decode

Needs only Python 3 (no packages):

```
sh decode/check.sh
```

Expected output:

```
f379r stream: identical to data/f379r/plaintext.txt (593 bytes)
f379r by-line: identical to data/f379r/plaintext-by-line.txt (700 bytes)
f379v stream: identical to data/f379v/plaintext.txt (573 bytes)
f379v by-line: identical to data/f379v/plaintext-by-line.txt (683 bytes)
f380r stream: identical to data/f380r/plaintext.txt (581 bytes)
f380r by-line: identical to data/f380r/plaintext-by-line.txt (684 bytes)
f380v stream: identical to data/f380v/plaintext.txt (597 bytes)
f380v by-line: identical to data/f380v/plaintext-by-line.txt (714 bytes)
f381r stream: identical to data/f381r/plaintext.txt (622 bytes)
f381r by-line: identical to data/f381r/plaintext-by-line.txt (734 bytes)
f381v stream: identical to data/f381v/plaintext.txt (329 bytes)
f381v by-line: identical to data/f381v/plaintext-by-line.txt (391 bytes)
all pages reproduced exactly
```

`plaintext.txt` and `plaintext-by-line.txt` were written by our own tools when the reading was made, so the check is a test of `decode.py` against an independent implementation. To read one page line by line: `python3 decode/decode.py data/f379r/key.json data/f379r/signs.txt --by-line`.

The measurement on known text can be recomputed with `python3 method/score_heldout.py`:

```
pass_a  227 / 238 reference signs read right -> sign accuracy 0.9538
pass_b  225 / 238 reference signs read right -> sign accuracy 0.9454
pass_c  220 / 238 reference signs read right -> sign accuracy 0.9244
vote    229 / 238 reference signs read right -> sign accuracy 0.9622
```

What cannot be repeated from this repository alone: Claude's sign readings themselves (they are recorded here, not re-run), and the dictionary and language model used for the value choice, word breaks, bits per letter and dictionary cover (built from our own period corpora).

## Credits

- **Satoshi Tomokiyo**, for the reconstruction of Matignon's Cipher-3, the catalogue of these letters, and the first published line of this despatch (<https://cryptiana.web.fc2.com/code/henryiii.htm>).
- **Bibliothèque nationale de France / Gallica**, for the manuscript images. Source gallica.bnf.fr / BnF.
- **Anthropic's Claude** (model Opus 5.5) was used as the sign reader, for the correction checks, for reading the calibration decipherment and the reference lines by eye, and for the English gist.

Prepared by Brett Burford, October 2026.

## Licence

- Text and data (everything except `decode/`, `method/score_heldout.py` and the images noted below): [Creative Commons Attribution 4.0 International](LICENSE) (CC BY 4.0).
- `decode/` and `method/score_heldout.py`: [MIT licence](decode/LICENSE).
- The image in `method/` (`sheet-v2.png`) is made of crops of BnF, Français 15572, f. 277r, from Gallica. It is not covered by CC BY: Gallica's terms allow free non-commercial reuse with the source line "Source gallica.bnf.fr / BnF"; commercial reuse needs the BnF's permission.
