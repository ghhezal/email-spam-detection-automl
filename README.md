# Email Spam Detection with Naive Bayes & AutoML (FLAML)

An end-to-end Machine Learning study on the **UCI Spambase Dataset**. This project compares a **Manual Gaussian Naive Bayes** classifier (built from scratch using NumPy) against automated tree-based models searched by **FLAML AutoML (LightGBM)**.

## Getting Started

### 1. Prerequisites

- Python 3.10+ (Tested on Python 3.12)
- Git

### 2. Clone the Repository

```bash
git clone https://github.com/ghhezal/email-spam-detection-automl.git
cd email-spam-detection-automl
```

### 3. Create & Activate Virtual Environment

- **Linux / macOS (Bash / Zsh):**
  **Bash**

  ```
  python -m venv .venv
  source .venv/bin/activate
  ```

- **Windows (Command Prompt - `cmd.exe`):**
  **DOS**

  ```
  python -m venv .venv
  .venv\Scripts\activate.bat
  ```

- **Windows (PowerShell):**
  **PowerShell**

  ```
  python -m venv .venv
  .venv\Scripts\Activate.ps1
  ```

### 4. Install Dependencies

**Bash**

```
pip install --upgrade pip
pip install -r requirements.txt
```

### 5. Run the Notebook

Launch Jupyter Lab or VS Code:

**Bash**

```
jupyter notebook notebooks/spam_detection_automl.ipynb
```

Select the `.venv` kernel to run the cells.

## Key Results

| **Model**                       | **Test Accuracy** | **Test F1-Score** | **Training / Search Time** |
| ------------------------------- | ----------------- | ----------------- | -------------------------- |
| **Manual Gaussian Naive Bayes** | 77.79%            | 77.87%            | \~0.009s                   |
| **FLAML AutoML (LightGBM)**     | **94.06%**        | **92.49%**        | 61.3s                      |
