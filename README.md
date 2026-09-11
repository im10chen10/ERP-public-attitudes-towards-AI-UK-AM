# Public Attitudes Towards AI Across Application Domains

This repository holds the code and aggregated statistical outputs for the ERP report *Public Attitudes Towards AI Across Application Domains: A Triangulation of Survey Data and Reddit Discussions*.

## Contents

`notebook/` contains the three Jupyter notebooks used in the analysis. `Subm_Ada_analysis.ipynb` covers all survey-based analysis (preprocessing, descriptive statistics, latent class analysis, multinomial logistic regression and both robustness checks). `Subm_Reddit_analysis.ipynb` includes Reddit corpus construction, sentiment scoring and cross-modal alignment. `submission_archive_anonymisation.ipynb` is a standalone script that produces an anonymised version of the Reddit archive.

`outputs/figures/` contains the ten figures used in the report. `outputs/aggregated_results/` contains the domain-level and class-level statistical summaries used as inputs to the alignment analysis. These files hold aggregated statistics only and contain no post text.

`technical_appendix.pdf` is the full technical appendix and describing how to reproduce result.

## Data

The raw survey file and the Reddit corpus need to be obtained separately before the notebooks can be run. See `data/README.md` for full instructions.

## Environment

The analysis was run in Python 3.11 under Jupyter Notebook. The three packages that materially affect the results are `stepmix` (3.0.0), `statsmodels` (0.14), and `scikit-learn` (1.4). Other packages used include `pandas`, `numpy`, `scipy`, `matplotlib`, `vaderSentiment`, `nltk` (with the `punkt_tab` tokeniser), and `requests`.

## Contact

For questions about this project or requests for access to the anonymised Reddit corpus, contact `im10yeah@gmail.com`.
