# Data access

The analysis uses two datasets, neither of which is included in this repository.

## Survey data

The survey data are from the Ada Lovelace Institute and the Alan Turing Institute's *Wave 2 2024/25: How do people feel about AI?*. They are hosted publicly at:

https://github.com/AdaLovelaceInstitute/wave-2---how-do-people-feel-about-AI-/blob/main/README.md

Download the raw CSV file and save it into this `data/` folder before running `Subm_Ada analysis.ipynb`. The notebook reads the file with Latin-1 encoding. The specific variables used are the sixteen attitude items (BenFR, ConFR, BenWB, ConWB, BenCancer, ConCancer, BenLoan, ConLoan, BenLLM, ConLLM, BenChatbot, ConChatbot, BenRoboCare, ConRoboCare, BenCar, ConCar) and the six demographic covariates (Cur_Sex, Cur_AgeCat, Cur_HEdQual, Cur_PartyID5, Cur_RClassGp, Cur_EconAct5).

## Reddit corpus

The Reddit corpus is not distributed in either raw or anonymised form here.

Two options are available for anyone wishing to work with the corpus.

The exact corpus used in the analysis, in anonymised form, can be requested by email at `im10yeah@gmail.com`.

Alternatively, the corpus can be reconstructed by running the retrieval code in the `Subm_Reddit analysis.ipynb` against the current Arctic Shift snapshot at `https://arctic-shift.photon-reddit.com`. The retrieval targets six subreddits (unitedkingdom, CasualUK, AskUK, UKPolitics, technology, artificial) over the twelve months from 2024-06-01 to 2025-06-01. The full keyword list is in Appendix B of the report. Because the archive continues to be updated, a reconstructed corpus will not be the same as original.
