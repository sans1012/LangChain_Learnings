# 🤝 Contributing Guide

This repository is primarily a personal learning repository.

However, contributions, suggestions, improvements, and discussions are always welcome.

---

# Development Setup

Follow the instructions in

```
SETUP.md
```

---

# Repository Structure

```
1-LangChain/
2-Lang-Graph/
Projects/
```

Each topic should be organized in its own folder.

---

# Coding Guidelines

## Python

- Follow PEP8
- Use meaningful variable names
- Add comments where necessary
- Prefer readability over clever code

---

## Jupyter Notebooks

Every notebook should contain

1. Title

2. Objective

3. Imports

4. Implementation

5. Observations

6. Summary

---

## File Naming

Use

```
01_prompt_templates.ipynb

02_chat_models.ipynb

03_output_parsers.ipynb
```

Avoid

```
Untitled.ipynb

new.ipynb

test.ipynb
```

---

# Folder Naming

Good

```
1-LangChain

2-Lang-Graph

Projects
```

Avoid

```
New Folder

temp

misc
```

---

# Git Workflow

Before starting

```bash
git pull
```

After changes

```bash
git status
```

```bash
git add .
```

```bash
git commit -m "Meaningful message"
```

```bash
git push
```

---

# Commit Message Convention

Examples

```
Added Prompt Templates notebook

Implemented LangGraph StateGraph example

Integrated Gemini API

Built first RAG pipeline

Added SQL Agent
```

Avoid

```
Update

Changes

Fixed

Testing
```

---

# Branch Naming

Examples

```
feature/rag

feature/langgraph

feature/mcp

bugfix/chromadb

docs/setup
```

---

# Adding Dependencies

Whenever adding a package

```bash
pip install package_name
```

Update

```
requirements.txt
```

---

# Environment Variables

Never commit

```
.env
```

Always use

```
.env.example
```

---

# Large Files

Avoid committing

- Virtual environments
- Model weights
- Large datasets
- Generated cache

Instead

Use

```
.gitignore
```

---

# Recommended Workflow

```
Pull

↓

Implement

↓

Test

↓

Commit

↓

Push
```

---

# Documentation

Whenever a new topic is completed

Update

- README.md
- CHANGELOG.md

---

# Thank You

Happy Learning 🚀
