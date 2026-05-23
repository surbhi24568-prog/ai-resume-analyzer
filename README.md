🤖 AI Resume Analyzer

A powerful, lightweight Python command-line utility that extracts data, scores, and provides structured feedback on resumes. Running entirely offline without requiring expensive API tokens, it analyzes formatting, contact presence, skill taxonomies, and action verb usage against custom scoring rules.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)





📁 Project Architecture
```text
ai-resume-analyzer/
├── src/
│   ├── __init__.py
│   └── analyzer.py         # Core extraction, tokenizing, and scoring engine
├── tests/
│   ├── __init__.py
│   └── test_analyzer.py    # Unit tests and continuous test logic (pytest)
├── sample_resumes/
│   └── sample_resume.txt   # Demo software engineering profile blueprint
├── outputs/                # Auto-generated JSON reports directory (Git-ignored)
├── .gitignore              # Standard exclusions (caches, virtualenvs, local PDFs)
├── LICENSE                 # Open-source MIT License
├── main.py                 # Core CLI runtime interface
└── requirements.txt        # Verified external packaging dependencies


