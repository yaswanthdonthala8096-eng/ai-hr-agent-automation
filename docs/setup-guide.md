# Setup Guide (n8n)

## Prerequisites
- n8n instance (cloud or self-hosted)
- Credentials configured:
  - Google Drive OAuth
  - Google Sheets OAuth
  - Gmail OAuth
  - OpenAI API
  - Google Gemini API

## Import Workflow
1. In n8n, go to Workflows → Import from File
2. Import `workflows/AI HR Agent.json`

## Configure
- Update Google Sheet ID and column mappings if needed
- Ensure the resume file is a PDF (required by Extract from File node)
- Set scoring thresholds in the IF nodes (example: 0.7 resume fit, 35/50 interview score)

## Run Test
1. Submit the form with a sample resume PDF
2. Confirm:
   - row created in Google Sheet
   - score generated
   - questionnaire generated
   - email sent based on outcome
