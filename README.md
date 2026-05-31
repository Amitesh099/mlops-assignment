# MLOps Assignment 1

## Objective

The objective of this project is to design and automate a complete machine learning workflow to predict Boston housing prices using classical machine learning models.

---

## Models Used

1. DecisionTreeRegressor
2. KernelRidge

---

## Project Structure

```text
mlops-assignment/
│
├── train.py
├── train2.py
├── misc.py
├── requirements.txt
├── README.md
└── .github/
    └── workflows/
        └── ci.yml
```

---

## Create Conda Environment

```bash
conda create -n mlops python=3.10 -y
conda activate mlops
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Decision Tree Model

```bash
python train.py
```

---

## Run Kernel Ridge Model

```bash
python train2.py
```

---

## GitHub Actions

A CI/CD workflow is configured using GitHub Actions.

Whenever code is pushed to the `kernelridge` branch:
- dependencies are installed automatically
- both ML models are executed
- model performance is displayed

---

## Results

| Model | MSE |
|------|------|
| Decision Tree | 10.41 |
| Kernel Ridge | 28.83 |

---

## Repository Branches

- main
- dtree
- kernelridge

---

## Technologies Used

- Python
- Scikit-learn
- Pandas
- NumPy
- Git
- GitHub Actions
- Conda
