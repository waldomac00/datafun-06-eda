# datafun-06-eda
**Author:** Michael J Moore  
**Date:** September 26, 2025  

---

## 📌 Overview
This repository is for **CC6.1: Start a Python EDA Project**.  
It follows the professional project initialization process described here:  
[Pro Analytics 01 – Project Initialization](https://github.com/denisecase/pro-analytics-01/tree/main/02-Project-Initialization)  

The goal is to practice **repeatable, professional workflows** for Python projects,  
using GitHub for version control and project publication.

---

## ⚙️ Initialization Process
Steps followed to initialize this project:

1. **Create repository in GitHub**  
   - Repo name: `datafun-06-eda`  
   - Initialized with default `README.md`

2. **Clone repo locally**
   ```bash
   cd ~/Repos
   git clone https://github.com/waldomac00/datafun-06-eda
   cd datafun-06-eda
   ```

3. **Add common project files**
   - `.gitignore` (ignores `.venv/`, `__pycache__/`, `*.sqlite`, `.DS_Store`, etc.)  
   - `requirements.txt` (tracks dependencies)

   Example `.gitignore` content:
   ```
   .venv/
   __pycache__/
   *.sqlite
   .DS_Store
   ```

4. **Commit and push changes**
   ```bash
   git add .
   git commit -m "Initialize project with gitignore and requirements.txt"
   git push origin main
   ```

5. **Create and activate virtual environment**

   **Windows PowerShell**
   ```bash
   py -3.12 -m venv .venv
   .venv\Scripts\Activate
   ```

   **Mac/Linux**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

---

## 📂 Project Structure
```
datafun-06-eda/
├── data/               # Datasets (CSV, JSON, etc.)
├── notebooks/          # Jupyter notebooks for analysis
├── src/                # Python source code
├── outputs/            # Generated charts, CSVs, summaries
├── .gitignore
├── requirements.txt
└── README.md
```

---

## ▶️ Repeatable Workflow
Reference: [Pro Analytics 01 – Repeatable Workflow](https://github.com/denisecase/pro-analytics-01/tree/main/03-repeatable-workflow)

### Activate virtual environment
```bash
# Windows
.venv\Scripts\Activate

# Mac/Linux
source .venv/bin/activate
```

### Install dependencies
```bash
pip install --upgrade pip setuptools wheel
pip install -r requirements.txt
```

Save dependencies:
```bash
pip freeze > requirements.txt
```

### Verify installation
```bash
python --version
pip list
jupyter lab
```

---

## 📊 Module Goal
In this module, you will:  

- Create a professional Python EDA project  
- Manage dependencies with `requirements.txt`  
- Use a clean, repeatable workflow for development  
- Load, explore, visualize, and analyze datasets with Python and Jupyter Notebooks  
- Produce charts and insights following the [datafun-06-spec](https://github.com/denisecase/datafun-06-spec)

---

## 📦 Initial Dependencies
The project starts with these packages (more may be added later):

- `jupyterlab`  
- `numpy`  
- `pandas`  
- `pyarrow`  
- `matplotlib`  
- `seaborn`  

Install with:
```bash
pip install -r requirements.txt
```

---

## ✅ Notes
- Always activate your `.venv` before running Python or Jupyter.  
- Always `git pull` before starting new work.  
- Commit early and often with clear messages.  

Example:
```bash
git pull
git add .
git commit -m "Add exploratory notebook"
git push origin main
```

---
