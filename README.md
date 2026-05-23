# 🤖 AI Resume Analyzer

A powerful, lightweight Python command-line utility that extracts data, scores, and provides structured feedback on resumes. Running entirely offline without requiring expensive API tokens, it analyzes formatting, contact presence, skill taxonomies, and action verb usage against custom scoring rules.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)



✨ Features

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







🔧 Deep Dive: How the Core Engine Works
[ Target Resume File ]
                 │
                 ▼
       [ Text Extraction Stage ] ──────► (Handles PDF, DOCX, or TXT structures)
                 │
                 ▼
       [ Pipeline Normalization ] ────► (Regex compilation & Keyword matching)
                 │
                 ├──► Contact Meta Engine (Name, Emails, Linked Profiles)
                 ├──► Section Auditor (Validates Summary, Experience, Projects)
                 ├──► Skill Categorizer (Maps against multi-tiered skill arrays)
                 └──► Action Verb & Metric Auditor (Scans language impact)
                 │
                 ▼
       [ Algorithmic Scoring Engine ] ─► (Applies 100-point weighted metrics)
     │
                 ▼
       [ Suggestion Matrix Engine ] ──► (Generates targeted delta feedback)
                 │
                 ▼
       [ Formatted Interface Interface / Save to JSON ]







📦 Installation & Setup
1.Clone the repository to your local workspace:
git clone [https://github.com/YOUR-USERNAME/ai-resume-analyzer.git](https://github.com/YOUR-USERNAME/ai-resume-analyzer.git)
cd ai-resume-analyzer


2.Spin up a clean Python virtual environment:
python -m venv venv
# On Windows environments:
venv\Scripts\activate
# On macOS/Linux environments:
source venv/bin/activate

3.Install dependencies:
pip install -r requirements.txt





🚀 Execution & Usage
You can interface directly with the tool using main.py. Pass your resume paths directly as positional arguments:

Standard Visual Report
python main.py sample_resumes/sample_resume.txt

Raw Structured JSON Payload output
python main.py sample_resumes/sample_resume.txt --json

Analyze and Save output report automatically to disk
python main.py sample_resumes/sample_resume.txt --save

Your report will compile instantly into a timestamped output document at ./outputs/report_YYYYMMDD_HHMMSS.json.







🧪 Running Unit Tests
The test infrastructure is pre-configured via pytest. To validate text handling, edge-case scores, dictionary mappings, and suggestion loops, execute:
pytest tests/test_analyzer.py -v





🛣️ Strategic Roadmap
. [ ] Job Description Mapping: Algorithmic comparison matching a target resume directly against user-defined Job Descriptions (JDs).

. [ ] Generative Refactoring UI: Integrating optional downstream LLM configurations (OpenAI GPT/Google Gemini APIs) for automated inline bullet point rewrites.

. [ ] Interactive Client Interface: Deploying a web frontend utilizing Streamlit or Flask for easy drag-and-drop resume uploading.

. [ ] ATS Optimization Profiles: Simulating basic Applicant Tracking System scanner behaviors to detect layout or structural compilation failures.



📝 License
Personal project — for personal use only.








