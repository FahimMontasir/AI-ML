# AI/ML Learning Journey Repository

This repository is my hands-on learning journey in **Python, Machine Learning, and Deep Learning**.

It is organized by topic and course stage, and includes notebooks, assignments, exam practice, and datasets. The goal is to make my progress easy to review for myself and useful for others who want to learn from practical examples.

## What This Repository Contains

- Foundational Python practice (`NumPy`, `Pandas`, data structures, problem solving)
- Data analysis and visualization practice (`Matplotlib`, `Seaborn`, `Plotly`)
- Applied machine learning workflows (EDA, preprocessing, regression, classification, evaluation)
- Deep learning theory + implementation with PyTorch (manual tensor pipeline, model training loop, hyperparameter comparison)

---

## Detailed Summary of What I Learned So Far

### 1) Python Foundations and Data Handling (`1-python/`)

### Core Python + Problem Solving

- Implemented basic Python exercises and logic-building tasks.
- Practiced object-oriented coding through a custom `LinkedList` implementation.

### NumPy Skills

- Created and inspected arrays (`dtype`, `ndim`, `shape`, `size`).
- Practiced array creation methods: `array`, `zeros`, `ones`, `arange`, `linspace`, random arrays, identity/diagonal matrices.
- Applied slicing, iteration (`nditer`), and basic vectorized operations.
- Solved assignment-style tasks using NumPy:
  - Max/min/mean calculations
  - Boolean filtering (e.g., age > 30)
  - Aggregations and transformations

### Pandas Skills

- Loaded CSV files and explored data with `head()`, `info()`, `describe()`, and `tail()`.
- Selected columns and filtered rows with conditions.
- Sorted and summarized tabular data.
- Applied real preprocessing operations:
  - Group-based missing value filling (e.g., salary by department median)
  - Conditional replacement using `loc`
  - Derived feature creation (e.g., `SalaryPerHour`)

### Data Visualization Skills

- Built visualizations using:
  - `Matplotlib` and `Seaborn` for histograms, countplots, pairplots, and heatmaps
  - `Plotly` for interactive grouped bar charts
- Learned how to format plots with titles, labels, legends, and readable layouts.

---

### 2) Machine Learning Practice (`2-ml/`)

### ML Problem Framing

- Identified target variables, features, and task types (classification vs regression).
- Practiced selecting useful columns and dropping noisy/high-cardinality columns when appropriate.

### Exploratory Data Analysis (EDA)

- Worked with real datasets like **Titanic**, **insurance**, and **loan** data.
- Performed:
  - Missing value analysis
  - Univariate and bivariate analysis
  - Correlation analysis and heatmaps
  - Target-wise categorical analysis

### Data Preprocessing

- Handled missing values with strategy-based choices (median/mode, dropping sparse columns like `Cabin`).
- Encoded categorical features using `OneHotEncoder` and label encoding.
- Applied feature scaling (`StandardScaler`, `RobustScaler`).
- Built clean model-ready datasets and verified no missing/non-numeric issues before training.

### Regression Models (Insurance Use Case)

- Trained and compared multiple models:
  - Multiple Linear Regression
  - Polynomial Regression
  - Support Vector Regression (SVR)
  - Random Forest Regressor
- Evaluated using:
  - RMSE
  - MAE
  - $R^2$
- Reviewed feature importance for interpretability.

### Classification Models (Loan/Titanic Style Use Cases)

- Prepared stratified train/test splits.
- Trained and evaluated:
  - Logistic Regression
  - Support Vector Machine (SVM)
  - Gaussian Naive Bayes
  - K-Nearest Neighbors (with K tuning)
  - Random Forest Classifier
- Used metrics and diagnostics:
  - Accuracy, Precision, Recall, F1
  - Confusion Matrix
  - ROC / AUC
  - Threshold effect on precision-recall tradeoff

### Exam-Level Applied Thinking

- Practiced robust statistics (median/IQR) and outlier detection.
- Applied Bayes theorem for real-world interpretation (PPV sensitivity to prevalence).
- Solved end-to-end pipeline questions with reasoning and step-by-step explanation.
- Performed residual analysis for regression model diagnostics.

---

### 3) Deep Learning (`3-dl/`)

### Deep Learning Theory (Final Exam Notebook)

- Studied and explained:
  - Backpropagation and chain rule
  - Weight/bias updates
  - Vanishing gradient problem and solutions
  - ANN architecture basics
  - ANN vs CNN comparison
  - Activation functions (Sigmoid, Tanh, ReLU)
  - Convolution and pooling operations
  - CNN shape calculations across layers

### Deep Learning Practice with PyTorch (Cost-of-Living Assignment)

- Implemented a **manual supervised learning pipeline** without `Dataset`/`DataLoader`.
- Prepared tabular data end-to-end:
  - Missing value handling with `SimpleImputer`
  - Feature scaling with `StandardScaler`
  - NumPy conversion and tensor conversion
  - Stratified train/test split
- Built a neural network with custom `nn.Module`.
- Selected and justified:
  - `BCEWithLogitsLoss` for binary classification
  - `Adam` optimizer
- Implemented full training loop:
  - Forward pass
  - Loss computation
  - Backward pass
  - Parameter update
  - Gradient reset
- Evaluated train/test accuracy and discussed overfitting/underfitting signals.
- Compared hyperparameter change effects (e.g., learning rate) on convergence and performance.

---

## Learning and Practice Habits I Followed

- Worked in notebook format with step-by-step explanations.
- Used clear markdown notes for reasoning, not just code outputs.
- Compared multiple models instead of stopping at one baseline.
- Used reproducibility settings (`random_state=42`, fixed seeds).
- Focused on both **implementation** and **interpretation** (not only metrics).

---

## Repository Structure (with Purpose)

```text
ai-ml/
├── README.md
├── requirements.txt
├── 1-python/
│   ├── matplotlib-seaborn/      # Visualization and employee dataset tasks
│   ├── numpy/                   # NumPy and Pandas fundamentals + assignments
│   ├── practice/                # Basic coding practice
│   └── problem-solving/         # Python problem solving exercises
├── 2-ml/
│   ├── ML_Mid_Term_Exam_2.ipynb # Midterm theory + applied ML coding
│   ├── assignment3/             # Supervised learning model comparison
│   └── Titanic/                 # EDA + preprocessing focused assignment
└── 3-dl/
   ├── DL_Final_Exam_Question.ipynb   # Deep learning theory-focused exam answers
   └── cost-of-living/                # PyTorch-based deep learning assignment
```

---

## Tech Stack Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Plotly
- Scikit-learn
- PyTorch

(All required packages are listed in `requirements.txt`.)

---

## Getting Started

### Prerequisites

- Python 3.8+
- `pip`

### Setup

1. Clone this repository.
2. Create and activate a virtual environment.
3. Install dependencies from `requirements.txt`.
4. Open notebooks with Jupyter/VS Code and run cells top-to-bottom.

---

## Who This Repo Is Useful For

- Beginners learning Python for data science
- Students practicing ML assignments and exam-style questions
- Anyone wanting notebook-based examples of EDA, preprocessing, model training, and evaluation

---

## Next Improvement Goals

- Add final comparison tables for all major models in one place.
- Add brief “key takeaways” at the end of each notebook.
- Add mini-project summaries with problem, approach, and results.

---

## Contributing

Feedback, suggestions, and improvements are welcome. If you want to contribute, feel free to open an issue or pull request.
