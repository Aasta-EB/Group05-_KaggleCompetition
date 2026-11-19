# NLI preprocessing
[Open the notebook in Colab](https://colab.research.google.com/github/Aasta-EB/Group05-_KaggleCompetition/blob/main/preprocessing/01_NLI_Preprocessing.ipynb).
The notebook includes the completed preprocessing run, results and plots. To rerun it, use Run all in Colab and upload the original competition ZIP when prompted.
Use train_clean.csv for training (9,667 rows) and validation_clean.csv for evaluation (2,453 rows). Keep the IDs in split_manifest.csv for every experiment. Fit TF-IDF and other learned transformations on training, then transform validation.
Use premise_clean and hypothesis_clean for text features. The raw text columns remain available for inspecting examples. test_clean.csv has the 5,195 unlabeled competition examples.
The summary, counts and similarity audit record the data checks. One of 200 sampled validation premises had similarity of at least 0.95 to a training premise.
Optional Block 1 model training is disabled by default. Its POS features cover English only. Model comparisons and Block 2 experiments still need to be run.
