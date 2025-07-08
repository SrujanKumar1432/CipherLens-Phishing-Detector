# Phishing Detection Algorithms

This repository provides a Python-based implementation to train and evaluate several machine learning models on phishing detection datasets. The script `run_algorithms.py` automates the process of running Neural Networks, Random Forests, and Support Vector Machines (SVM) on your data and prints out key performance metrics for each model.

---

## Features

- **Multiple Algorithms**: Runs Neural Network, Random Forest, and SVM classifiers.
- **Metrics Calculation**: Computes accuracy, sensitivity, specificity, and F1-score for each run.
- **Easy Dataset Integration**: Just place your dataset and label files in CSV format.

---

## Getting Started

### Prerequisites

- Python 3.x
- Required Python packages:
  - pandas
  - numpy
  - scikit-learn

Install dependencies using:

```bash
pip install pandas numpy scikit-learn
```

### Input Files

- `Dataset.csv` : The feature dataset.
- `Target_Labels.csv` : The corresponding class labels.

> Both files should be in the same directory as `run_algorithms.py`.

### Running the Script

```bash
python run_algorithms.py
```

You will see output for each classifier, along with runtime information.

---

## Example Output

```
running neural networks...
runtime = 2.34 seconds

running random forests...
runtime = 0.87 seconds

running support vector machines...
runtime = 1.12 seconds

runtime = 4.33 seconds
```

---

## Screenshots

Screenshots of running the script and sample outputs are provided below.

### 1. Script Output in Terminal

![Screenshot 1 - Script Output](screenshots/screenshot1.png)

### 2. Example Dataset Files

![Screenshot 2 - Dataset CSV](screenshots/screenshot2.png)

---

## Customization

- You can change the test/train split by modifying `test_size` in the `main()` function.
- To use different datasets, replace `Dataset.csv` and `Target_Labels.csv` with your own files (ensure the format matches).

---

## Notes

- The script uses scikit-learn's classic APIs. For newer versions, replace `sklearn.cross_validation` with `sklearn.model_selection`.
- Make sure your CSV files are clean and free from missing values.

---

## License

This project is for educational purposes.
