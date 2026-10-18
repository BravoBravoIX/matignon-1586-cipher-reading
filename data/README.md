# Data

Per page (`f379r` = f. 379 recto, `f379v` = f. 379 verso, … `f381v`):

| file | contents |
|---|---|
| `signs.txt` | the sign names as read, one manuscript line per row: line number, a tab, the signs separated by spaces. Names are visual names from the reference sheet (`../method/sheet-v2.png`), plus `q`, `v`, `oo`, `Lp`, `Lx2` (described in `../method/prompt.txt`); `x` = a sign on no row of the sheet; `?` = a sign not made out |
| `key.json` | the key as a table (`pipeline[0].table`: each name's value, `type`, confidence and origin), and under `pipeline[0].choices` the value taken at every occurrence of the two-valued signs `y`, `yv` and `8`, in reading order |
| `plaintext.txt` | the literal plaintext as one stream (signs without a value as `[?name]`), as written by our tool when the reading was made |
| `plaintext-by-line.txt` | the same, one manuscript line per row (signs without a value as `·`) |
| `reading.json` | per sign position: the names given by the reader passes, most voted first; the passes; the corrections applied |
| `corrections.json` | the rule for corrections and the changes applied on this page (line, 0-based position, old and new name) |
| `controls.json` | the page decoded as read, with its signs shuffled (seeds 1-3), and its last fifth on its own: bits per letter and dictionary cover |

`key-cipher3.json`: the key with the origin of every value (`T` Tomokiyo's table, `E` alignment with the 1586 decipherment, `E?` doubtful).

`known-text/`: the calibration material. `f279r-decipherment.txt`, `f280r-decipherment.txt` are our readings by eye of the decipherment made at the time (fr. 15572 ff. 279r, 280r); `ref-278r-l12-18.txt` the reference signs of the held-out lines; `heldout-278r-l10-26.txt` the known text of f. 278r lines 10-26; `stageB/` the three passes and the vote on f. 278r; `scores/` the recorded scores; `em-key-v2.json` the values given by the alignment of our reading of ff. 277r-278r with the decipherment (the `E` origin).

Line numbers of f. 381v start at 0 here; in `../reading/ff379-381-french.md` they start at 1.
