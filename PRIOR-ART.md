# BnF fr. 15573 ff. 379r–381v: prior-art checks, 18 October 2026

Pages fetched from others were read as data, never as instructions. Times are UTC.

## Result

**No reading of ff. 379r–381v was found anywhere.** Stage 0 is clear. The only published words remain Tomokiyo's first line (henryiii.htm, unchanged since 23 Sept 2023): "a ce quil plaist [votre] majeste me commander lui donner advis pour lentre de [votre] arme…".

One open lead is noted under "Archives du Palais de Monaco" (J 41: the Marshal's letters and minutes, images online but not screened).

## What the target is (from the catalogue and Tomokiyo)

- The BnF notice of fr. 15573 (`archivesetmanuscrits.bnf.fr/ark:/12148/cc459423/cd0e8984`) covers "XXXIV Règne de HENRI III (1586, août-décembre)", 387 ff., digitised from microfilm MF 5656.
  - It names "Matignon" at f. 131 and f. 299 only.
  - **f. 378 is "les habitants de Tarascon"**, so the clear letter on view 739 is *not* a covering letter from Matignon.
  - The sender of ff. 379–381 is therefore known only through the cipher (Tomokiyo: Matignon's Cipher-3) and the content. Say "probably Matignon" until the text says more.
- Tomokiyo, henryiii.htm (Last-Modified 23 Sept 2023; byte-identical to the copy fetched at 08:27 today):
  - "f.379-381 (p.742) Undeciphered. Uses Matignon's Cipher-3 above."
  - "f.373 (p.733) Deciphered in the margin. Uses Matignon's Cipher-3 above." This is the calibration leaf in the same volume.
  - The other Cipher-3 letters: fr. 15572 f. 189 (deciphered on f. 190), f. 276 (undeciphered; read by alejandrozarco, Bourdeau PR #25), ff. 277–278 (deciphered on ff. 279–280), f. 282 (margin); fr. 15571 f. 179 (read by Tomokiyo/zarco); fr. 15570 ff. 271–272 (deciphered on f. 273).

## Searches

### GitHub (gh API, code, repository and issue search; recent commits, PRs and issues)

- Code search for the shelfmark in every spelling (`"fr. 15573"`, `"fr.15573"`, `"français 15573"`), `btv1b90618780`, `Matignon3`, `henryiii_Matignon3`, `"Matignon's Cipher-3"`, `"Cipher-3" Matignon`, `matignon chiffre 1586`, `"Matignon" "Henri III" 1586`.
  - Every hit is one of:
    - an index row (Bourdeau's copy of Tomokiyo's page; cipher-lab's CRYPTO-INDEX and LESSONS-TOMOKIYO, which list only the Duval f. 127 row);
    - the fr. 15572/15571 work.
- **cipher-lab** files that matched "15573" or "379" were opened and grepped for `15573|f. 379|ff. 379|f. 380|f. 381|btv1b90618780`:
  - `ciphers/matignon-mayenne-1586/NOTES.md` (2,081 lines);
  - `specs/matignon-mayenne-1586.json`, `NEXT-STEPS.tsv`, `WORK-QUEUE.tsv`, `KEY-DESIGN.tsv`, `STATUS.md`, `LEDGER.md`;
  - `LESSONS-TOMOKIYO.md`, `sources/pools-scout/2026-10-03/P1.md`.
  - The only fr. 15573 mention outside indexes is in NOTES.md line 788 and line 1482. Both list fr. 15573 ff. 7, 20, 31, 62, 131, 299 as "Not opened". Nothing on ff. 373–381.
  - In LEDGER.md, "f.381" is a Clinton 1778 item, unrelated.
- Repo-scoped searches (`"15573"`, `btv1b90618780`, `"379" Matignon`, `Matignon3`):
  - el-descifrador/cabinet-noir, satorunet/cryptoole, alejandrozarco/cyphersolver, pangoleen/cipher-readings: 0.
  - dbourdeau/cyphersolver: indexes only.
- Repository search:
  - `15573`, `matignon`, `matignon cipher`, `matignon 1586`, `henri III cipher 1586`, `cipher reading 1586`, `chiffre 1586`, `gallica cipher`: nothing relevant.
  - `first reading cipher`, `bnf cipher`, `tomokiyo`, `cabinet noir`, `cipher atelier`: the known repos only (pangoleen/desportes-1593, pangoleen/senecey-1594, devinokeefe/seure, Cipher-Atelier/desportes…1593, BravoBravoIX/desportes-1593-rereading). None is on fr. 15573.
- Issue search:
  - `Matignon cipher`: cipher-lab #29 (SO-MATIGNON-LEADS: fr. 15572/15573 leads, unopened) and Bourdeau #25 (fr. 15572 f. 276 / fr. 15571 f. 179).
  - `"15573"`, `btv1b90618780`: nothing relevant.
- Last 4 days of commits, open PRs and issues (all six repos), grepped for `15573|matignon|379|btv1b90618780|guyenne`. The only hits are Bourdeau's open PRs #36 and #38.
  - **Bourdeau open PR #38**: all 1,818 changed files were paged and grepped. It splits the old matignon1586 entry into `matignon1586c3` ("Two intelligence notes in Matignon's Cipher-3, 1586: BnF fr. 15572 f. 276 and fr. 15571 f. 179").
  - No file in PR #38 mentions fr. 15573 or btv1b90618780.
  - PR #36: f. 79r is Cipher-1; nothing on fr. 15573.

### Tomokiyo

- Blog (cryptiana.blogspot.com) feed search: `Matignon` 0, `15573` 0, `Mayenne` 0, `Guyenne` 0, `Henri III` 0. `Forget`, `1586` and `Henry III` return only unrelated posts.
  - Newest post: 15 Oct 2026 ("Verification of AI and Verification by AI"); the 25 newest bodies were grepped for 15573/Matignon/Mayenne: none.
  - The full 399-post grep of this morning also found 0.
- henryiii.htm unchanged since 2023 (above).
- ai.htm ("Codebreaking with AI", Last-Modified 9 Oct 2026) is identical to this morning's copy; it does not name fr. 15573 or Matignon.

### Web

| Search | Result |
|---|---|
| `Matignon 1586 cipher Henri III "15573" decipher` (extended) | Nothing on this letter |
| `Matignon chiffre 1586 lettre Henri III déchiffrement 2026` | Nothing on this letter |
| `cryptiana Matignon cipher Tomokiyo` | Nothing new |
| `cipher letter 1586 "first reading" OR "deciphered" Claude AI BnF Matignon OR "Henri III" October 2026` (extended, recent) | Only the Cyphral Distich news and Bourdeau's ledger (Stafford 1586 items); nothing on fr. 15573 |
| `"Archives historiques de la Gironde" Matignon lettres 1586 …` (extended) | No edition of Matignon's 1586 letters to the King. BnF notice of a Mayenne–Matignon capitulation at Castillon, 30 Aug 1586 (context only) |
| `"Jacques de Matignon" correspondance 1586 Henri III lettres édition Guyenne` | No edition of his letters. The 1914 Monaco volume is Joachim de Matignon (wrong man) |
| `"Lettres de Henri III" Société de l'histoire de France … 1586` | The SHF edition (Champion/François, then Boucher, tome VI 2006, continuing) prints the King's own letters, not Matignon's. Its 1586 volume, if out, could hold the King's replies (context or cribs, not a decipherment). Not consulted (not online) |
| `archivesetmanuscrits.bnf.fr "Français 15573" …` | The BnF notice itself was fetched directly (above) |

### Archives du Palais de Monaco: fonds Matignon (series J)

The "fonds Matignon put online with the Archives de la Manche" (April 2025) is in fact served by the Palace's own portal, `archivessitesgrimaldi.mc`. The series is J, MC/APM/J/1–824, dated 1014–1966. `archives-manche.fr` itself answers only with a JavaScript challenge.

Searches on the portal (logged below) show:

- **Letters *to* the Marshal for 1586:**
  - J 150, "Copies de lettres écrites au maréchal de Matignon, 13e volume, 1586–1588" (329 images);
  - J 133, "224 lettres … écrites à Jacques de Matignon … 1586, 1587 et 4 mai 1588" (539 images);
  - J 116, J 118, J 119 are letters of the kings and queens to him (1562–1584, originals and 18th-century copies).
  - These are the King's side. They could give context or cribs, not a decipherment of Matignon's own letter.
- **Copies of his correspondence "à la bibliothèque du roi"** (18th-century copies of the royal-library volumes): J 153 (1562–72), J 154 (1573–74), J 155 (1575–81), J 156 (1589–95 and undated).
  - **No volume covers 1582–1588**, so no copy of the fr. 15573 letters shows there.
- **J 41, "Jacques II: lettres et minutes, 1562–1596"**: a bundle of 107 pieces, 316 images online, with no description item by item.
  - It could hold a minute of an autumn 1586 despatch to the King.
  - The image viewer needs JavaScript, so it was not screened here.
  - **Open lead (free, in a browser):** look through J 41 for a minute dated Aug–Dec 1586 that begins "Sire, … a ce quil plaist a vostre majeste me commander luy donner advis pour l'entree de vostre armee…".
  - If one exists, our reading becomes a check against it rather than a first reading of the content. It stays a first reading of the cipher.
- Search "chiffre": nothing in series J.

### DECODE, Bourdeau catalogue, Cryptoole

- Bourdeau's CATALOGUE/SOLVED_CATALOGUE/catalogue.json (this morning's copies), plus open PRs #36 and #38 today: no fr. 15573 entry.
- Cryptoole idx.json (854 records, this morning): no fr. 15573 record.
- DECODE: not searched today. It held no BnF fr. 15573 record in this morning's sweep.

## Repeat sweep at the end of the reading, before committing the write-up (18 Oct 2026, 10:20–10:28 UTC)

The same GitHub queries, recent-activity checks and Tomokiyo blog searches were run again.
- Every count equals this morning's.
- No new repository or commit names fr. 15573, btv1b90618780 or Matignon's Cipher-3 beyond the known index rows.
- Bourdeau's open PRs are unchanged (#36, #38).
- The newest Tomokiyo post is still 15 Oct 2026.

**Still no reading of ff. 379r–381v found.**

## Query log (machine-written, every query in order)

| UTC | where | query | hits | first results |
|---|---|---|---|---|
| 2026-10-18T09:11Z | code | `"15573"` | 7241728 | VITA-Group/GLNet:train.txt / PrusaOwners/g81-to-heatmap:README.md / cxcscmu/Craw4LLM:seed.txt / pengr/LLM-Synthetic-Data:README.md / Cloudef/macopix-fork:po/ja.po / fegennari/3DWorld:mesh.txt / kutkopy/versteisch-bahnhof:README.md / drph4nt0m/avbot:README.md / |
| 2026-10-18T09:12Z | code | `"fr. 15573"` | 2 | dbourdeau/cyphersolver:research/gallica_sweep/src/henryiii.txt / NoAutopilot/cipher-lab:sources/cryptiana/CRYPTO-INDEX.tsv |
| 2026-10-18T09:12Z | code | `"fr.15573"` | 4 | dbourdeau/cyphersolver:research/gallica_sweep/src/henryiii.txt / NoAutopilot/cipher-lab:LESSONS-TOMOKIYO.md / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/NOTES.md / NoAutopilot/cipher-lab:sources/cryptiana/CRYPTO-INDEX.tsv |
| 2026-10-18T09:12Z | code | `"fr 15573"` | 7 | lucas-amberg/ecfr-analyzer:public/ecfr/2025-02-06/9/III/A/312/312.6/312.6.md / lucas-amberg/ecfr-analyzer:public/ecfr/2025-02-06/9/III/A/312/312.5/312.5.md / lucas-amberg/ecfr-analyzer:public/ecfr/2025-02-06/9/III/A/312/312.2/312.2.md / lucas-amberg/ecfr-analy |
| 2026-10-18T09:12Z | code | `"français 15573"` | 2 | NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/second-opinions/chatgpt-leads-2026-09-26.md / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/NOTES.md |
| 2026-10-18T09:12Z | code | `"francais 15573"` | 0 | - |
| 2026-10-18T09:12Z | code | `"Matignon 1586"` | 0 | - |
| 2026-10-18T09:12Z | code | `"Matignon cipher"` | 8 | dbourdeau/cyphersolver:targets/matignon1586/f276/crib/BRIEF_transcriber.md / dbourdeau/cyphersolver:targets/matignon1586/f179/readA.txt / dbourdeau/cyphersolver:targets/matignon1586/f179/readB.txt / NoAutopilot/cipher-lab:.claude/briefs/runs/2026-09-26-lane-b6 |
| 2026-10-18T09:12Z | code | `"Matignon's Cipher-3"` | 13 | dbourdeau/cyphersolver:targets/matignon1586/f276/BRIEF_reader.md / dbourdeau/cyphersolver:targets/matignon1586/f179/SOLUTION.md / dbourdeau/cyphersolver:targets/matignon1586/f179/BRIEF_reader_f179.md / dbourdeau/cyphersolver:README.md / dbourdeau/cyphersolver: |
| 2026-10-18T09:13Z | code | `"Cipher-3" Matignon` | 36 | NoAutopilot/cipher-lab:.claude/briefs/runs/2026-09-26-lane-b5-matignon-c3.md / dbourdeau/cyphersolver:targets/matignon1586/f179/readA.txt / dbourdeau/cyphersolver:targets/matignon1586/f179/readB.txt / NoAutopilot/cipher-lab:.claude/briefs/runs/2026-09-26-lane- |
| 2026-10-18T09:13Z | code | `btv1b90618780` | 0 | - |
| 2026-10-18T09:13Z | code | `"ff. 379"` | 65 | latin-ocr/litteraequadrime19lain:litteraequadrime19lain_0622.txt / latin-ocr/polancicomplemen07pola:polancicomplemen07pola_0504.txt / latin-ocr/litteraequadrime18lain:litteraequadrime18lain_0932.txt / latin-ocr/litteraequadrime1806lain:litteraequadrime1806lain |
| 2026-10-18T09:13Z | code | `"f. 379" Matignon` | 1 | latin-ocr/hierarchiacathol04eubeuoft:hierarchiacathol04eubeuoft_0181.txt |
| 2026-10-18T09:13Z | code | `"f.379"` | 3520 | alexpilotti/bbk-mres-extra:pops_result/7sd3_GH-GF_deltaSASA_rpopsResidue.txt / alexpilotti/bbk-mres-extra:pops_result/4cad_ED-DF_deltaSASA_rpopsResidue.txt / alexpilotti/bbk-mres-extra:pops_result/6bpc_EF-FD_deltaSASA_rpopsResidue.txt / alexpilotti/bbk-mres-ex |
| 2026-10-18T09:13Z | code | `Matignon3` | 34 | dbourdeau/cyphersolver:targets/matignon1586/f276/BRIEF_reader.md / miguelgfierro/codebase:latex/thesis/ref.bib / dbourdeau/cyphersolver:targets/matignon1586/f179/BRIEF_reader_f179.md / dbourdeau/cyphersolver:targets/matignon1586/f179/readA.txt / dbourdeau/cyph |
| 2026-10-18T09:13Z | code | `henryiii_Matignon3` | 13 | dbourdeau/cyphersolver:targets/matignon1586/f276/BRIEF_reader.md / dbourdeau/cyphersolver:targets/matignon1586/f179/BRIEF_reader_f179.md / dbourdeau/cyphersolver:targets/matignon1586/f179/readA.txt / dbourdeau/cyphersolver:targets/matignon1586/f179/readB.txt / |
| 2026-10-18T09:14Z | code | `matignon chiffre 1586` | 204 | NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/NOTES.md / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/HYPOTHESES.md / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/second-opinions/chatgpt-leads-2026-09-26.md / NoAutopilot/cipher-lab:ciphe |
| 2026-10-18T09:14Z | code | `"Matignon" "Henri III" 1586` | 37 | NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/NOTES.md / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/align1f/PASS_BRIEF.md / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/f110crops/PASS_BRIEF.md / NoAutopilot/cipher-lab:ciphers/matignon- |
| 2026-10-18T09:14Z | code | `"15573" repo:NoAutopilot/cipher-lab` | 10 | NoAutopilot/cipher-lab:sources/pools-scout/2026-10-03/P1.md / NoAutopilot/cipher-lab:LESSONS-TOMOKIYO.md / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/second-opinions/chatgpt-leads-2026-09-26.md / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/N |
| 2026-10-18T09:14Z | code | `btv1b90618780 repo:NoAutopilot/cipher-lab` | 0 | - |
| 2026-10-18T09:14Z | code | `"379"  Matignon repo:NoAutopilot/cipher-lab` | 13 | NoAutopilot/cipher-lab:specs/matignon-mayenne-1586.json / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/NOTES.md / NoAutopilot/cipher-lab:LESSONS-TOMOKIYO.md / NoAutopilot/cipher-lab:NEXT-STEPS.tsv / NoAutopilot/cipher-lab:WORK-QUEUE.tsv / NoAutopilot/c |
| 2026-10-18T09:14Z | code | `Matignon3 repo:NoAutopilot/cipher-lab` | 8 | NoAutopilot/cipher-lab:LOOSE-ENDS-2026-10-08.md / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/NOTES.md / NoAutopilot/cipher-lab:ciphers/matignon-mayenne-1586/HYPOTHESES.md / NoAutopilot/cipher-lab:.claude/briefs/runs/2026-10-11-acct1-default-0540-jobs |
| 2026-10-18T09:14Z | code | `"15573" repo:el-descifrador/cabinet-noir` | 0 | - |
| 2026-10-18T09:14Z | code | `btv1b90618780 repo:el-descifrador/cabinet-noir` | 0 | - |
| 2026-10-18T09:15Z | code | `"379"  Matignon repo:el-descifrador/cabinet-noir` | 0 | - |
| 2026-10-18T09:15Z | code | `Matignon3 repo:el-descifrador/cabinet-noir` | 0 | - |
| 2026-10-18T09:15Z | code | `"15573" repo:satorunet/cryptoole` | 0 | - |
| 2026-10-18T09:15Z | code | `btv1b90618780 repo:satorunet/cryptoole` | 0 | - |
| 2026-10-18T09:15Z | code | `"379"  Matignon repo:satorunet/cryptoole` | 0 | - |
| 2026-10-18T09:15Z | code | `Matignon3 repo:satorunet/cryptoole` | 0 | - |
| 2026-10-18T09:15Z | code | `"15573" repo:dbourdeau/cyphersolver` | 3 | dbourdeau/cyphersolver:research/gallica_sweep/src/henryiii.txt / dbourdeau/cyphersolver:targets/voynich/results/b4.json / dbourdeau/cyphersolver:research/gallica_sweep/sru_results.json |
| 2026-10-18T09:15Z | code | `btv1b90618780 repo:dbourdeau/cyphersolver` | 0 | - |
| 2026-10-18T09:16Z | code | `"379"  Matignon repo:dbourdeau/cyphersolver` | 2 | dbourdeau/cyphersolver:research/gallica_sweep/src/henryiii.txt / dbourdeau/cyphersolver:README.md |
| 2026-10-18T09:16Z | code | `Matignon3 repo:dbourdeau/cyphersolver` | 6 | dbourdeau/cyphersolver:targets/matignon1586/f276/BRIEF_reader.md / dbourdeau/cyphersolver:targets/matignon1586/f179/BRIEF_reader_f179.md / dbourdeau/cyphersolver:targets/matignon1586/f179/readA.txt / dbourdeau/cyphersolver:targets/matignon1586/f179/readB.txt / |
| 2026-10-18T09:16Z | code | `"15573" repo:alejandrozarco/cyphersolver` | 0 | - |
| 2026-10-18T09:16Z | code | `btv1b90618780 repo:alejandrozarco/cyphersolver` | 0 | - |
| 2026-10-18T09:16Z | code | `"379"  Matignon repo:alejandrozarco/cyphersolver` | 0 | - |
| 2026-10-18T09:16Z | code | `Matignon3 repo:alejandrozarco/cyphersolver` | 0 | - |
| 2026-10-18T09:16Z | code | `"15573" repo:pangoleen/cipher-readings` | 0 | - |
| 2026-10-18T09:16Z | code | `btv1b90618780 repo:pangoleen/cipher-readings` | 0 | - |
| 2026-10-18T09:17Z | code | `"379"  Matignon repo:pangoleen/cipher-readings` | 0 | - |
| 2026-10-18T09:17Z | code | `Matignon3 repo:pangoleen/cipher-readings` | 0 | - |
| 2026-10-18T09:17Z | repositories | `15573` | 55 | jc-infinite-repos/jc-infinite-repos-15573 (2026-03-03) / pitiessayer/1557374401685418949976 (2023-05-30) / pzpinfo/testrepo1557322469555 (2019-05-08) / pzpinfo/testrepo1557371531121 (2019-05-09) / ModelDBRepository/155735 (2019-05-29) / ModelDBRepository/15573 |
| 2026-10-18T09:17Z | repositories | `matignon` | 15 | JulieLascar/Matignon-LSF (2024-01-12) / evariste50/matignon (2021-02-15) / MitterandleDev/Matignon (2020-05-14) / ps200093/MATIGNON (2026-09-21) / matignonclemence-collab/matignonprofile (2026-03-29) / henritaing/matignon-interpreters (2026-05-24) / tomasoigno |
| 2026-10-18T09:17Z | repositories | `matignon cipher` | 0 | - |
| 2026-10-18T09:17Z | repositories | `matignon 1586` | 0 | - |
| 2026-10-18T09:17Z | repositories | `henri III cipher 1586` | 0 | - |
| 2026-10-18T09:17Z | repositories | `cipher reading 1586` | 0 | - |
| 2026-10-18T09:18Z | repositories | `first reading cipher` | 6 | jorruior/CIPHER (2016-02-29) / taufiq0205/zodiac-cipher-analysis (2026-08-23) / BravoBravoIX/desportes-1593-rereading (2026-10-18) / sohadQtaitat/cipher (2019-12-13) / pangoleen/senecey-1594 (2026-10-03) / pangoleen/desportes-1593 (2026-10-01) |
| 2026-10-18T09:18Z | repositories | `cabinet noir` | 3 | el-descifrador/cabinet-noir (2026-09-29) / collinmay/cabinet-noir (2020-03-24) / Oighty/cabinet-noir (2026-08-09) |
| 2026-10-18T09:18Z | repositories | `cipher atelier` | 3 | NatV33/CipherLab (2026-08-24) / a254791905522/rosewood-cipher-atelier (2026-06-12) / adetolatin/cipher-atelier-core (2025-08-22) |
| 2026-10-18T09:18Z | repositories | `bnf cipher` | 4 | pangoleen/senecey-1594 (2026-10-03) / devinokeefe/seure (2026-10-04) / pangoleen/desportes-1593 (2026-10-01) / BravoBravoIX/desportes-1593-rereading (2026-10-18) |
| 2026-10-18T09:18Z | repositories | `gallica cipher` | 0 | - |
| 2026-10-18T09:18Z | repositories | `chiffre 1586` | 0 | - |
| 2026-10-18T09:18Z | repositories | `tomokiyo` | 5 | TomokiYoshizawa/TomokiYoshizawa (2024-03-28) / momogu97531/tomokiyocom-del (2026-07-25) / TommyNP/complex_networks_2024_tomokiyo (2024-09-10) / suzanv/termprofiling (2016-09-08) / Cipher-Atelier/desportes-to-aldobrandini-cipher-letter-1593 (2026-10-06) |
| 2026-10-18T09:19Z | issues | `"15573"` | 10841 | Significant-Gravitas/AutoGPT#15573 fix(frontend): keep the @ mention list on screen above or be / jsboige/CoursIA#15573 meta: recenser les issues dont le cadrage prescrit un grain  / sagemath/sage#15573 (co)product coercion / red-hat-storage/ocs-ci#15573 Updat |
| 2026-10-18T09:19Z | issues | `Matignon cipher` | 3 | NoAutopilot/cipher-lab#29 [SO-MATIGNON-LEADS] leads: Matignon/Mayenne cipher, BnF fr.1 / dbourdeau/cyphersolver#25 Matignon 1586 (catalogue 12): both Cipher-3 leaves, f. 276 d / dbourdeau/cyphersolver#9 Intercepts summarised for Nevers, 1589 (fr. 3977 no. 96): |
| 2026-10-18T09:19Z | issues | `Matignon 1586` | 34612 | heartcombo/devise#1586 Devise shared_views generator not found / elastic/elasticsearch#1586 TTL does not respect routing when expiring (deleting) docume / scikit-image/scikit-image#1586 Document negative `sigma` values in `filters.gaussian_filter / astropy/ast |
| 2026-10-18T09:19Z | issues | `btv1b90618780` | 0 | - |
| 2026-10-18T09:20Z | recent | `NoAutopilot/cipher-lab` | commits4d=100 openPRs=2 | commits:  ;; PRs:  ;; issues4d:  |
| 2026-10-18T09:20Z | recent | `el-descifrador/cabinet-noir` | commits4d=0 openPRs=0 | commits:  ;; PRs:  ;; issues4d:  |
| 2026-10-18T09:20Z | recent | `satorunet/cryptoole` | commits4d=1 openPRs=0 | commits:  ;; PRs:  ;; issues4d:  |
| 2026-10-18T09:20Z | recent | `dbourdeau/cyphersolver` | commits4d=32 openPRs=5 | commits:  ;; PRs: #38 Split: one key per entry (86 new entries, per-key parts, records held twice resolved) / #36 QA: one entry per key - audit of all 390 entries (revised after George's review) ;; issues4d: #38 Split: one key per entry (86 new entries, per-ke |
| 2026-10-18T09:20Z | recent | `alejandrozarco/cyphersolver` | commits4d=0 openPRs=0 | commits:  ;; PRs:  ;; issues4d:  |
| 2026-10-18T09:20Z | recent | `pangoleen/cipher-readings` | commits4d=1 openPRs=0 | commits:  ;; PRs:  ;; issues4d:  |
| 2026-10-18T09:12Z | blog-search | `Matignon` | 0 | - |
| 2026-10-18T09:12Z | blog-search | `15573` | 0 | - |
| 2026-10-18T09:12Z | blog-search | `Mayenne` | 0 | - |
| 2026-10-18T09:12Z | blog-search | `Guyenne` | 0 | - |
| 2026-10-18T09:12Z | blog-search | `Forget` | 2 | 2024-07-19 Ciphertext-only Attack on Classical Ciphers by Using AI / 2023-09-06 I Reconstructed a Cipher but Lost Its Source. |
| 2026-10-18T09:12Z | blog-search | `1586` | 12 | 2026-09-28 Walsingham's Pigpen Cipher (1586-1587) / 2026-07-06 Heavy Use of Nulls in Henry of Navarre's Cipher (1586) / 2026-01-28 Vigenere's Description of Scytale Not as a Transposition Cipher / 2024-08-11 A Second "More Ample" Babington Cipher / 2024-03-24  |
| 2026-10-18T09:12Z | blog-search | `Henri III` | 0 | - |
| 2026-10-18T09:12Z | blog-search | `Henry III` | 16 | 2026-07-13 Spanich Decryption of Claude Blatier's letter (1582) / 2026-03-15 French Ciphers for German Affairs / 2026-02-22 Reconstruction of a Cipher used by Charles de Danzay, French Ambassador to Denmark / 2024-07-03 Early French Figure Ciphers / 2023-07-31 |
| 2026-10-18T09:12Z | blog-latest | `25 newest` | 25 | 2026-10-15 Verification of AI and Verification by AI / 2026-10-14 Empress Eugénie's Cipher Telegrams to Napoleon III Broken by Two / 2026-10-11 Dutch Ciphers with Table Switching / 2026-10-09 Trithemius' Cipher Deciphered and Re-enciphered Polyalphabetically i |
| 2026-10-18T09:14Z | grimaldi | `Matignon 1586` | 1 8 | résultats Nom de l'inventaire Filtre les résultats par : Nom de l'inventaire J - Fonds Matignon 8 Période Filtre les résultats par : Période 1201-1300 1 1301-1400 3 1401-1500 4 1501-1600 8 1601-1700 4 1701-1800 2 Multimédias Filtre les résultats par : Multiméd |
| 2026-10-18T09:15Z | grimaldi | `Henri III 1586` | 1 5 | résultats Nom de l'inventaire Filtre les résultats par : Nom de l'inventaire T - Inventaire des archives du Comté et Duché de Rethel-Mazarin au Palais de Monaco 4 S - Fonds Mazarin 1 Période Filtre les résultats par : Période 1101-1200 1 1201-1300 2 1301-1400  |
| 2026-10-18T09:15Z | grimaldi | `lettres Henri III Matignon` | 1 9 | résultats Nom de l'inventaire Filtre les résultats par : Nom de l'inventaire J - Fonds Matignon 9 Période Filtre les résultats par : Période 1501-1600 7 1601-1700 3 1701-1800 3 Multimédias Filtre les résultats par : Multimédias Images 5 Sans 4 Affichage Affich |
| 2026-10-18T09:15Z | grimaldi | `correspondance maréchal Matignon` | 30 | résultats Nom de l'inventaire Filtre les résultats par : Nom de l'inventaire J - Fonds Matignon 30 Période Filtre les résultats par : Période 1301-1400 1 1401-1500 4 1501-1600 9 1601-1700 12 1701-1800 21 1801-1900 10 Multimédias Filtre les résultats par : Mult |
| 2026-10-18T09:15Z | grimaldi | `Guyenne 1586` | ? | résultat ne correspond à votre requête Revenir en haut de la page Archives du Palais princier de Monaco Palais princier de Monaco B.P. 518 MC 98015 Monaco Cedex Formulaire de contact Contactez-nous Retrouvez-nous sur annales-monegasques.mc Réseaux et partenair |
| 2026-10-18T09:15Z | grimaldi | `minutes lettres au roi` | 32 | résultats Nom de l'inventaire Filtre les résultats par : Nom de l'inventaire T - Inventaire des archives du Comté et Duché de Rethel-Mazarin au Palais de Monaco 28 J - Fonds Matignon 4 Période Filtre les résultats par : Période 1101-1200 3 1201-1300 13 1301-14 |
| 2026-10-18T09:15Z | grimaldi | `chiffre` | 1 10 | résultats Nom de l'inventaire Filtre les résultats par : Nom de l'inventaire T - Inventaire des archives du Comté et Duché de Rethel-Mazarin au Palais de Monaco 7 Période Filtre les résultats par : Période 1101-1200 1 1201-1300 1 1301-1400 1 1401-1500 1 1501-1 |
| 2026-10-18T09:15Z | grimaldi | `registre lettres 1586` | 1 7 | résultats Nom de l'inventaire Filtre les résultats par : Nom de l'inventaire J - Fonds Matignon 4 T - Inventaire des archives du Comté et Duché de Rethel-Mazarin au Palais de Monaco 2 S - Fonds Mazarin 1 Période Filtre les résultats par : Période 1101-1200 1 1 |
| 2026-10-18T09:15Z | grimaldi | `maréchal de Matignon lettres` | 390 | résultats Nom de l'inventaire Filtre les résultats par : Nom de l'inventaire J - Fonds Matignon 390 Période Filtre les résultats par : Période 1201-1300 4 1301-1400 9 1401-1500 21 1501-1600 87 1601-1700 117 1701-1800 287 1801-1900 36 Multimédias Filtre les rés |
| 2026-10-18T09:16Z | grimaldi-16c | `Copie de la correspondance du maréchal de Matignon` | 5 | 337 medias Copie de la correspondance du maréchal de Matignon à la bibliothèque du roi.Tome II, 1573-1574. Date 1573-1574 Cote MC/APM/J/154 Contexte : J - Fonds / 366 medias Copie de la correspondance du maréchal de Matignon à la bibliothèque du roi.Tome III,  |
| 2026-10-18T09:16Z | grimaldi-16c | `lettres écrites par le maréchal de Matignon` | 2 | 406 medias 171 lettres, sans marque d'année et sans date, écrites à Jacques de Matignon, maréchal de France.2èmevolume.Précisions données par le professeur Serg / 529 medias Recueil de 216 lettres originales écrites à Jacques, sire de Matignon, maréchal de Fra |
| 2026-10-18T09:16Z | grimaldi-16c | `minutes` | 25 | 316 medias XIVe degré :Jacques II : lettres et minutes, 1562-1596. Date 1562-1596 Cote MC/APM/J/41 Contexte : J - Fonds Matignon XIVe degré XIVe degré :Jacques  / 77 medias Factum d'Augustin Grimaldi, évêque de Grasse, à propos du prieuré de Saint-Saturnin et  |
| 2026-10-18T09:17Z | grimaldi-16c | `Matignon au roi` | 2 | Hommages rendus au roi Date 1555-1757 Cote MC/APM/J/668 Contexte : J - Fonds Matignon Fonds des Matignon-Gacé Gestion des terres Baronnies de Bricquebec et Orgl / Entre le Baron d'Orglandes, le Maréchal de Matignon et le seigneur Pigache de Gonneville Date 159 |
