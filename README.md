# AI-Jobs-Applier-Agent

Python-based workflow that generates tailord resumes and cover letters and also pre-fills application forms to save effort and time

LLM: GPT4o

Key components

1. Master Resume & Cover Letter Template
- Both files in .txt format for easy parsing
- Cover letter as a dynamic template with placeholders (e.g., <CompanyName>, <PositionTitle>, <KeySkills>) and logic to populate those fields dynamically to match job descriptions

2. Parsing Job Descriptions
- Automation configured to parse job descriptions from LinkedIn, Indeed, and BuiltIn, and then extract relevant details for tailoring the resume and cover letter

3. Automating Application Portals
- Scripts that use Selenium and RPA tools to log in, fill out forms, and upload the tailored documents on Workday, Greenhouse and other portals

4. Pipeline Overview
- Input: Job descriptions, ymaster resume, and a dynamic cover letter template
- Processing: Parse job descriptions, tailor resumes/letters, and save drafts
- Output: Automatically apply on supported portals (or notify you to confirm applications)
