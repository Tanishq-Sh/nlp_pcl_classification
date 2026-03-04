# Patronizing and Condescending Language (PCL) Detection

This project focuses on detecting Patronizing and Condescending Language in text, a task from SemEval. The repository contains code for data preprocessing, model training, and prediction.

## Project Structure

```
.
├── BestModel/
│   └── best_model.ipynb        # Jupyter notebook for the best performing model.
├── StrongBaselineModel/
│   └── strong_baseline_model.ipynb # Jupyter notebook for a strong baseline model.
├── data/
│   ├── dontpatronizeme_pcl.tsv     # Main dataset file.
│   ├── train_semeval_parids-labels.csv # Training data labels.
│   ├── dev_semeval_parids-labels.csv   # Development data labels.
│   └── task4_test.tsv            # Unlabeled test data.
├── model_files/
│   ├── baseline_weighting_model/ # Saved files for a baseline model.
│   └── best_model_class_weighting_model/ # Saved files for the best model.
├── predictions/
│   ├── best_model_preds.csv      # Predictions from the best model on the dev set.
│   └── strong_baseline_model_preds.csv # Predictions from the baseline model on the dev set.
├── dev.txt                     # Predictions for the development set.
├── test.txt                    # Predictions for the test set.
├── requirements.txt            # Python dependencies for this project.
└── README.md                   # This file.
```

## Models

- **`BestModel`**: This directory contains the implementation of the best performing model, which appears to be a RoBERTa-based classifier with class weighting to handle data imbalance.
- **`StrongBaselineModel`**: This directory contains a strong baseline for comparison.

## How to Run

1.  **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```
2.  **Run the notebooks**:
    - Open and run the cells in `BestModel/best_model.ipynb` to train the best model and generate predictions.
    - Open and run the cells in `StrongBaselineModel/strong_baseline_model.ipynb` to work with the baseline model.

The final predictions for the official test set are saved in `test.txt`.
