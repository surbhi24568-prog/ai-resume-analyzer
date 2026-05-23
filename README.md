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

## ⚡ Features

* 📄 **Multi-Format Parsing** — Instantly decodes text from **PDF**, **DOCX**, and **TXT** files safely without system crashes.
* 📋 **Contact Information Harvesting** — Extracts target metadata including Name, Email, Phone, and social links using optimized regex expressions.
* 🌐 **Profile Validation** — Automatically verifies the presence of active developer links like **GitHub** and **LinkedIn** profiles.
* 🗺️ **Categorized Skill Detection** — Automatically tracks and maps matching text strings against an integrated **6-domain technical skill taxonomy database**.
* 📑 **Section Architecture Auditing** — Simulates ATS scanning behavior by verifying the presence of foundational resume components (Summary, Experience, Projects, etc.).
* 💪 **Action Verb Diagnostics** — Scans and counts high-impact professional terminology while flagging weak description language.
* 📈 **Quantified Impact Analytics** — Employs custom numerical pattern-matching to track data points, metrics, and percentages ($X\%$ reduction, $Yk+$ requests).
* 🏆 **Weighted Performance Scoring** — Generates a deterministic performance rating based on an exact **100-point weighted architectural algorithm**.
* 🎓 **Academic Letter Grading** — Instantly calculates and returns a standardized letter grade status ranking from **A down to F**.
* 💡 **Context-Aware Suggestion Matrix** — Evaluates missing document vectors to output customized, rule-based improvement checklists.
* 💻 **Dual-Stream Output Modes** — Streams visually striking, colorized terminal grids or exports raw structured **JSON objects** seamlessly.
* 💾 **Automated Report Logging** — Generates and dumps clean, timestamped analysis payloads directly to your local file outputs directory via `--save` flags.
* 🧪 **Automated Testing Suite** — Comes pre-configured with a dedicated **Pytest automation matrix** to ensure structural reliability across formatting updates.

