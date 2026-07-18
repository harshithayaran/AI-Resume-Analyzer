# AI-Resume-Analyzer
AI Resume Analyzer is an LLM-powered application that helps recruiters and job seekers evaluate how well a resume matches a job description.

The application extracts text from PDF files, sends the resume and job description to a Large Language Model (Groq Llama 3.3 70B), receives structured JSON output, validates it using Pydantic, and displays an easy-to-read skill analysis report.

## Features
- Read Resume PDF
- Read Job Description PDF
- Extract text using PyPDF
- Compare resume against job description
- Calculate Overall Match Percentage
- Identify Matching Skills
- Identify Missing Skills
- Highlight Candidate Strengths
- Highlight Candidate Weaknesses
- Suggest Skill Improvements
- Structured JSON output
- Pydantic validation
- Secure API key management using .env

  ## Tech Stack
- Python
- Groq API
- Llama 3.3 70B Versatile
- Pydantic
- PyPDF
- python-dotenv
- JSON

- ## Future Improvements
- Streamlit Web App
- Upload Resume from UI
- DOCX Support
- ATS Score Calculation
- Keyword Highlighting
- Multiple Resume Comparison
- Recruiter Dashboard
- OpenAI & Gemini Support
- Export Analysis to PDF
- RAG-powered Skill Recommendations

## Prerequisites
- Python 3.11+
- Groq API Key
- Internet Connection
- 
# 🚀 How to Run the Project

## 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/AI-Resume-Analyzer.git
cd AI-Resume-Analyzer
```
## 2. Create a Virtual Environment
Using `uv`:
```bash
uv venv
```
Activate it:

### Windows

```bash
.venv\Scripts\activate
```

### macOS/Linux

```bash
source .venv/bin/activate
```

---

## 3. Install Dependencies

```bash
uv add groq python-dotenv pypdf pydantic
```

## 4. Create a `.env` File

Create a `.env` file in the project root.

```env
GROQ_API_KEY=your_groq_api_key_here
```

---

## 5. Add Your PDFs

Update the file paths in the code or place your files in the desired directory.

Example:

```python
resume_path = r"C:\Users\YourName\Resume.pdf"

job_description_path = r"C:\Users\YourName\JobDescription.pdf"
```

---

## 6. Run the Project

```bash
python resume_checker.py
```

or with `uv`:

```bash
uv run python resume_checker.py
```

---

## Example Output

```
Overall Match: 82%

Matching Skills:
- Python
- SQL
- Machine Learning

Missing Skills:
- Docker
- Kubernetes

Strengths:
- Strong problem-solving skills
- Good programming fundamentals

Weaknesses:
- Limited cloud experience

Suggestions:
- Learn Docker
- Learn Kubernetes
- Build deployment projects
```

