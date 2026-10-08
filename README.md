# The mixed subjects design

Notebook for the EOS Masterclass (8 October 2026, David Broska). It estimates the treatment effect of one survey experiment three ways: with GPT-4 predictions only (silicon subjects), with human subjects only, and with both combined through prediction-powered inference (mixed subjects).

## Run
- Locally: `pip install numpy pandas matplotlib ppi-python`, then open `mixed_subjects_design.ipynb`.
- Google Colab: open the notebook from this repository, run `!pip install ppi-python`, and upload `data/connors.csv` into a `data/` folder.

## Data
`data/connors.csv` has one row per participant in two arms of the TESS experiment by Connors (2023, *Public Opinion Quarterly*, Study 4): `treated` (1 = friends reminder, 0 = control), `Y` (rating of Republicans, 0-100) and `Yhat` (GPT-4's predicted rating for a person with the same demographics in the same condition). It is derived from the replication archive of Ashokkumar, Hewitt, Ghezae & Willer (2026, *Nature*; Code Ocean, doi:10.24433/CO.6384242.v1).

## More details

This notebook applies the mixed subjects design from:

Broska, D., Howes, M., & van Loon, A. (2025). The Mixed Subjects Design: Treating Large Language Models as Potentially Informative Observations. *Sociological Methods & Research*, 54(3), 1074–1109. [https://doi.org/10.1177/00491241251326865](https://journals.sagepub.com/doi/full/10.1177/00491241251326865)

Replication code and data for the paper: [github.com/davidbroska/MixedSubjects](https://github.com/davidbroska/MixedSubjects)
