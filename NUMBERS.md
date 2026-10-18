# Where the numbers come from

Every number in [README.md](README.md) and [method/README.md](method/README.md), and the file in this repository it is taken from. They are written into the README by the script that assembles this repository, from the records made when the work was done (18 October 2026), not typed by hand.

| number | meaning | source in this repository |
|---|---|---|
| 127 lines, 2837 signs; per-page lines and signs | size of the reading | rows and sign names of `data/<page>/signs.txt` |
| 0.831, 0.8641, 0.8516, 0.8362, 0.8547, 0.8508 | share of positions where all three passes agree, ff. 379r … 381v | `data/<page>/reading.json` `all_agree_share` |
| 3, 6, 5, 5, 6, 0 (in all 25) | corrections applied per page | `data/<page>/corrections.json` `applied` |
| 10 per page; 60 looked at | correction proposals | `data/<page>/corrections.json` `rule` |
| 238 signs | reference signs of fr. 15572 f. 278r lines 12–18 | `data/known-text/scores/*.score.json` `ref_signs`; `data/known-text/ref-278r-l12-18.txt` |
| 0.9538 / 0.9454 / 0.9244 | sign accuracy of passes a / b / c | `data/known-text/scores/f278r-pass_a.score.json`, `-pass_b`, `-pass_c` `accuracy`; recomputed by `method/score_heldout.py` |
| 0.962 | sign accuracy of the vote (229 / 238) | `data/known-text/scores/f278r-vote.score.json` `accuracy` (0.9622); recomputed by `method/score_heldout.py` |
| 0.9328 | the same, strict (first accepted name only) | `data/known-text/scores/f278r-vote.strict.score.json` `accuracy`; `method/score_heldout.py --strict` |
| 0.87 | all three passes agree on the calibration page | our stage B record (not in this repository) |
| bits per letter, dictionary cover, shuffled seeds 1–3, held-out last fifth | controls per page | `data/<page>/controls.json` `reading`, `shuffled_seed1`–`3`, `held_out_last_fifth` |
| 2.65 bits per letter | the calibration decipherment text itself, same model | our stage C record (not in this repository) |
| 50 sign shapes, 2–5 examples each | reference sheet v2 | `method/sheet-v2.json` |
| piece widths and enlargements of the passes | reader passes | `data/<page>/reading.json` `passes` |
| byte counts in the check output | sizes of `data/<page>/plaintext.txt` and `plaintext-by-line.txt` | `sh decode/check.sh` |
| Gallica views 740–745, 739; fr. 15572 views 286, 288, 289, 290 | image locations | our fetch records; the links in the README |
| 18 October 2026, 10:20–10:28 UTC | dates of the prior-art searches | [PRIOR-ART.md](PRIOR-ART.md) |
