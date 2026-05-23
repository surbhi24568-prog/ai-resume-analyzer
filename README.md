# 🤖 AI Resume Analyzer

A powerful, lightweight Python command-line utility that extracts data, scores, and provides structured feedback on resumes. Running entirely offline without requiring expensive API tokens, it analyzes formatting, contact presence, skill taxonomies, and action verb usage against custom scoring rules.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)

---

## ✨ Features

- 📄 **Multi-Format Support** — Built-in structural parsing for PDF (`pdfplumber`), Word Documents (`python-docx`), and plain text (`.txt`).
- 📋 **Automated Contact Extraction** — Identifies applicant name, email, phone number, and professional profiles (LinkedIn, GitHub).
- 🛠️ **Categorized Skill Detection** — Automatically maps text against a comprehensive taxonomy covering:
  - Programming Languages
  - Web Frameworks
  - Databases
  - Cloud & DevOps
  - Data & Machine Learning
  - Essential Soft Skills
- 💪 **Action Verb Audit** — Audits the quality of description language by flagging weak items and validating impactful action items.
- 📊 **Quantified Impact Evaluation** — Analyzes bullet points using natural language logic to detect performance metrics, rewarding resumes backed by data and statistics.
- 🏆 **100-Point Weighted Scoring System** — Automatically calculates a global score coupled with a standardized letter grade (`A` through `F`).
- 💡 **Actionable Optimization Gaps** — Provides clear, conditional feedback loops highlighting missing technical fields, weak verbs, or missing contact links.
- 💾 **Dual-Mode Outputs** — Output pretty terminal tables or parse clean `JSON` payloads for easy upstream API ingestion.
