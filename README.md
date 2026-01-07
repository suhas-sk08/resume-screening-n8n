# 📄 AI-Powered Resume Screening Automation (n8n)

## 🔍 Overview
An AI-driven resume screening system built using **n8n** to automate the end-to-end hiring workflow.  
The system automatically collects resumes, extracts candidate information, evaluates them against job requirements, and assigns relevance scores—reducing manual screening effort and improving hiring efficiency.

---

## 🚀 Features
- 📩 Automated resume intake (Gmail / Google Drive / Upload trigger)
- 📄 Resume parsing (PDF / DOCX)
- 🤖 AI-based resume evaluation using LLMs
- 🧠 Skill and experience matching with job descriptions
- 📊 Candidate scoring and ranking
- 📁 Structured result storage (Google Sheets / Database)
- 🔔 Automated shortlisting and notifications

---

## 🔄 Workflow
1. Resume received via Gmail or upload
2. File parsing and text extraction
3. AI-powered resume analysis
4. Skill & JD matching
5. Candidate scoring
6. Shortlisting and data storage

---

## ⚙️ n8n Nodes Used
- Gmail Trigger / Webhook
- Binary File Handler
- PDF/Text Extractor
- AI (LLM) Node
- Function Node (Scoring Logic)
- Google Sheets / Database Node
- IF / Switch Nodes

---

## 📊 Scoring Logic (Sample)
| Criteria        | Weight |
|-----------------|--------|
| Skill Match     | 40%    |
| Experience      | 30%    |
| Keyword Match   | 20%    |
| Education       | 10%    |

---

## 🧪 Sample Output
```json
{
  "name": "John Doe",
  "email": "john.doe@email.com",
  "skills": ["React", "Node.js", "SQL"],
  "experience": "3 Years",
  "score": 82,
  "status": "Shortlisted"
}

