# Resume Analyzer AI Agent (n8n + OpenAI + Google Sheets)

### Problem
HR teams and recruiters often spend hours reviewing resumes manually. This process is slow, repetitive, and inconsistent — especially when handling hundreds of candidates.

### Solution (n8n Workflow)
This agent automates resume screening by:
- **Resume Intake**: Collects resumes directly from Gmail or Google Drive.
- **File Handling**: Extracts text from PDF/DOCX files.
- **AI Processing**: Uses OpenAI to identify skills, education, and work experience.
- **Information Extraction**: Structures candidate details into fields (Name, Skills, Education, Experience).
- **Scoring**: Applies a code-based scoring system (e.g., skill match, years of experience).
- **Data Logging**: Appends results into Google Sheets for easy filtering & reporting.

### Result
- Reduces time-to-shortlist by 70%.
- Produces consistent, bias-reduced candidate scores.
- Provides a searchable structured database of resumes.

---

### ⚙️ Stack
- **n8n** (automation platform)
- **OpenAI Chat Model** (AI-based resume parsing & scoring)
- **Google Drive / Gmail** (resume source)
- **Google Sheets** (structured storage of parsed resumes)

---

### 🚀 How to Run (Demo)
1. Import `workflow.json` into n8n (this export is sanitized; no credentials included).
2. Configure credentials: Gmail/Google Drive + OpenAI + Google Sheets.
3. Upload or forward resumes into the Gmail/Drive folder.
4. Run the workflow — extracted details and scores will appear in Google Sheets.

---

### 📂 Repo Structure
```
/  
├── README.md              # Documentation  
├── workflow.json          # Sanitized n8n export (no secrets)  
├── /screenshots           # Workflow diagram & sample outputs  
└── LICENSE                # MIT License  
```

---

### 🖼️ Screenshots
- Workflow diagram (n8n nodes: Gmail → Drive → Extract → OpenAI → Sheets)
- Example parsed resume data in Google Sheets

---

### 🔒 Notes on Credentials & Safety
- This repo does **not** include any API keys or credentials.
- Configure OpenAI/Gmail/Drive/Sheets inside your own n8n instance.
- Replace placeholder sheet IDs and folder paths with your own.
