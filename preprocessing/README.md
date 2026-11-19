# NLI preprocessing

[Open the notebook in Colab](https://colab.research.google.com/github/Aasta-EB/Group05-_KaggleCompetition/blob/main/preprocessing/01_NLI_Preprocessing.ipynb).

The notebook includes the preprocessing results and plots. To rerun it in Colab, use Run all and upload the original competition ZIP when prompted.

Use train_clean.csv for training and validation_clean.csv for the local model comparison. The split has 9,667 training and 2,453 validation examples. Keep the IDs in split_manifest.csv for every experiment. Fit TF-IDF and other learned transformations on training, then transform validation.

test_clean.csv contains the 5,195 unlabeled test examples. The premise_clean and hypothesis_clean columns contain the text to use for features. The original text columns are kept alongside them for reviewing examples.

The summary, language counts and sampled similarity audit document the checks from this run. One of the 200 sampled validation rows had premise similarity of at least 0.95 to a training premise.

The optional Block 1 baseline cells are included with training disabled. Their POS features cover English only. This notebook completes data preparation. Model training and the Block 2 experiments remain to be run.
