# ⚙️ Development Setup Guide

This document explains how to set up the development environment for this repository from scratch.

---

# Requirements

- Python 3.11
- Git
- VS Code

---

# Clone Repository

```bash
git clone https://github.com/sans1012/LangChain_Learnings.git
```

```bash
cd LangChain_Learnings
```

---

# Create Virtual Environment

Windows

```bash
py -3.11 -m venv ai_env
```

Activate

```bash
.\ai_env\Scripts\activate
```

Linux/Mac

```bash
python3.11 -m venv ai_env
```

```bash
source ai_env/bin/activate
```

---

# Upgrade Pip

```bash
python -m pip install --upgrade pip
```

```bash
python -m pip install --upgrade setuptools wheel
```

---

# Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Jupyter Setup

Install

```bash
pip install notebook jupyterlab ipykernel
```

Register kernel

```bash
python -m ipykernel install --user --name ai_env --display-name "Python (AI_ENV)"
```

Open VS Code

Select

```
Python (AI_ENV)
```

Verify

```python
import sys

print(sys.executable)
```

Expected

```
...\ai_env\Scripts\python.exe
```

---

# Environment Variables

Create

```
.env
```

Example

```
GEMINI_API_KEY=

GROQ_API_KEY=

LANGCHAIN_API_KEY=
```

Load

```python
from dotenv import load_dotenv

load_dotenv()
```

Access

```python
import os

os.getenv("GEMINI_API_KEY")
```

---

# Installing New Packages

```bash
pip install package_name
```

Update requirements

```bash
pip freeze > requirements.txt
```

---

# Updating Packages

```bash
pip install --upgrade package_name
```

---

# Remove Package

```bash
pip uninstall package_name
```

---

# Useful Pip Commands

Installed packages

```bash
pip list
```

Package details

```bash
pip show langchain
```

Python version

```bash
python --version
```

Pip version

```bash
pip --version
```

Current interpreter

```python
import sys

print(sys.executable)
```

---

# Git Setup

Configure Git

```bash
git config --global user.name "Your Name"
```

```bash
git config --global user.email "your_email@example.com"
```

---

# Daily Workflow

Fetch latest changes

```bash
git pull
```

Check status

```bash
git status
```

Stage files

```bash
git add .
```

Commit

```bash
git commit -m "Meaningful commit message"
```

Push

```bash
git push
```

---

# .gitignore

The following are intentionally ignored:

```
ai_env/
.venv/
venv/
.env
__pycache__/
.ipynb_checkpoints/
.vscode/
```

---

# Troubleshooting

## ModuleNotFoundError

Usually means the package is not installed in the active environment.

Check

```python
import sys
print(sys.executable)
```

Install

```bash
pip install package_name
```

Restart Jupyter Kernel.

---

## Access Denied During pip Install

Run

```bash
python -m pip install --upgrade pip
```

or

```bash
pip install --user package_name
```

---

## Wrong Python Version

Check

```bash
python --version
```

or

```bash
py -3.11 --version
```

---

## Verify Installed Packages

```bash
pip list
```

---

# Recommended Folder Structure

```
LangChain_Learnings
│
├── ai_env
├── 1-LangChain
├── 2-Lang-Graph
├── Projects
├── requirements.txt
├── README.md
├── SETUP.md
├── .gitignore
└── .env
```

---

Happy Learning! 🚀