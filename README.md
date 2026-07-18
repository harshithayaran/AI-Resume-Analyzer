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
