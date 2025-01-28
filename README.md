# AI-Jobs-Applier-Agent

Python-based workflow that generates tailord resumes and cover letters and also pre-fills application forms to save effort and time

LLM: GPT4o

Key components

1. Master Resume & Cover Letter Template
- Both files in .txt format for easy parsing int standard JSON or YAML formats
- Cover letter as a dynamic template with placeholders (<CompanyName>, <PositionTitle>, <KeySkills>) and logic to populate those fields dynamically to match job descriptions
- CL template variations with pre-defined sections to empahsize experience and skills specific to industries 

2. Job Description Extraction
Automation configured to...
- Parse job descriptions from LinkedIn, Indeed, and BuiltIn, etc.
- And then extract relevant details for tailoring the resume and cover letter

3. Auto-aplication on Job Portals
- Scripts that use Selenium and RPA tools to log in, fill out forms and upload the tailored CVs and CLs on Workday, Greenhouse and other portals
Uses the following
- Selenium for navigating and filling application portals (like Workday and Greenhouse) via Robotic Process Automation (RPA)
- NLP tools or Pandas to auto-select relevant achievements or projects based on job descriptions 
- OpenAI for text customization (e.g., adapting templates to job descriptions)

4. Pipeline Overview
- Input: Job descriptions, master resume, and a dynamic cover letter template
- Processing: Parse job descriptions, tailor resumes/letters, and save drafts
- Output: Automatically apply on supported portals (or notify you to confirm applications)
