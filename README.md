# AI HR Agent (n8n) – Agentic AI Recruitment Automation

An end-to-end AI HR automation workflow built in **n8n** that:
- Collects candidate applications via form
- Uploads & parses resumes (PDF)
- Scores Resume vs Job Description using an LLM
- Generates a 5-question screening questionnaire
- Evaluates candidate answers and decides next step
- Logs results to Google Sheets
- Sends rejection or interview-invite emails automatically

## Workflow Stages
1. Candidate Form Submission (name, email, phone, resume)
2. Resume Upload to Google Drive + PDF Text Extraction
3. JD vs Resume Scoring (LLM) → pass/fail threshold
4. Auto-generated Screening Questions (LLM)
5. Candidate Answers Form
6. Answer Evaluation + Total Score (LLM) → pass/fail threshold
7. Google Sheets logging + Email automation

## Tech Stack
- n8n
- OpenAI API (resume scoring + question generation)
- Google Gemini API (answer evaluation)
- Google Drive (resume storage)
- Google Sheets (candidate tracking)
- Gmail (candidate communication)

## Files
- `workflows/AI HR Agent.json` – n8n workflow export
- `docs/setup-guide.md` – setup and credentials steps

## Author
Yaswanth Donthala
