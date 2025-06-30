# Automated Job Apply & Resume Tailoring System

This project automates the process of applying to jobs by:

- Scraping job listings (currently stubbed with sample data)
- Tailoring your resume to fit each job using OpenAI's GPT-4o
- Saving the customized resumes as individual text files

---

## Project Structure

automated_job_applier/
├── main.py # Main script to run the workflow
├── resume_tailor.py # Module to rewrite resume using OpenAI API
├── job_scraper.py # Stub module returning sample job listings
├── config.py # Stores your OpenAI API key
├── master_resume.txt # Your base resume in plain text format
└── data/
└── tailored_resumes/ # Folder where tailored resumes are saved

---

## Getting Started

### 1. Clone the repository or create project folder

```bash
git clone https://github.com/yourusername/automated_job_applier.git
cd automated_job_applier
Or create the folder and files manually as above.

2. Install dependencies
Requires Python 3.7+ and OpenAI Python package:

bash
pip install openai
3. Add your OpenAI API key
Open config.py and set your API key:

python
OPENAI_API_KEY = 'your-openai-api-key-here'
You can generate your key here: OpenAI API keys

4. Add your resume
Paste your plain text resume into:


master_resume.txt
5. Run the script

bash
python main.py
You should see output like:

bash
Saved tailored resume for 'Cybersecurity Analyst' at data/tailored_resumes/resume_1_Cybersecurity_Analyst.txt
Saved tailored resume for 'Information Security Specialist' at data/tailored_resumes/resume_2_Information_Security_Specialist.txt
Current Limitations
Job listings are currently sample/stub data, no live scraping yet.

Outputs resumes as plain text files only.

Resume input must be plain text.

Planned Improvements
Real job scraping from job sites (Indeed, LinkedIn, etc.)

AI-generated cover letters

Resume export to PDF or Word documents

User-friendly web or desktop interface

Automate job application submissions

Disclaimer
This is a prototype for educational and personal use. Always review AI-generated resumes carefully before sending to employers.

Contributions & Contact
Feel free to fork, submit issues, or request features
