
# AI Resume Analyzer with Generative AI

Introduction

This project presents an intelligent AI-powered application designed for in-depth resume analysis using Retrieval-Augmented Generation (RAG), Large Language Models (LLMs), and OpenAI’s capabilities. It summarizes resumes, highlights strengths and areas for improvement, and suggests suitable job titles tailored to a user's profile. Additionally, it integrates Selenium to automatically extract valuable job-related information from LinkedIn, including company names, positions, locations, job URLs, and full job descriptions. This tool streamlines the job-seeking process by offering actionable, data-driven insights to help users strengthen their career prospects.

Table of Contents

1. Core Technologies and Skills
2. Setup Instructions
3. How to Use
4. Application Features
5. Contributing Guidelines
6. License
7. Contact Information

Core Technologies and Skills

* Python
* NumPy & Pandas
* LangChain
* Large Language Models (LLMs)
* Retrieval-Augmented Generation (RAG)
* OpenAI API
* Selenium WebDriver
* AWS
* Hugging Face
* Streamlit

Installation

To set up the application, install the required dependencies using pip:

```python
pip install numpy
pip install pandas
pip install streamlit
pip install streamlit_option_menu
pip install streamlit_extras
pip install PyPDF2
pip install langchain
pip install openai
pip install tiktoken
pip install faiss-cpu
pip install selenium
```

Application Features

User-Friendly Design:

* The AI Resume Analyzer offers a smooth user experience by allowing easy resume uploads and API key input. The interface is intuitive and beginner-friendly.
* It leverages PyPDF2 to efficiently extract textual content from uploaded resumes, serving as the starting point for further analysis.

Advanced Text Processing with LangChain:

* The tool utilizes LangChain to intelligently split long text sections into manageable, overlapping chunks—improving the semantic accuracy of resume parsing.
* This chunking approach helps generate targeted recommendations for resume enhancement.

Seamless Integration with OpenAI & FAISS:

* By securely connecting to OpenAI via user-provided API keys, the system enables high-level language analysis.
* FAISS (Facebook AI Similarity Search) transforms both resume content and job queries into vector formats, enabling quick and relevant content retrieval.

Optimized Document Retrieval with RAG:

* The system ranks and selects the Top K most relevant chunks based on similarity to the user query, ensuring only the most contextually important text is processed.
* These selected chunks are analyzed using ChatGPT 3.5 Turbo, generating accurate and personalized feedback.

Powerful Q\&A Pipeline:

* The question-answering pipeline merges retrieved content and user queries to provide focused, informative answers.
* The LLM leverages contextual understanding to generate high-quality outputs based on relevant extracted content.

Detailed Resume Evaluation:

* Summary: Generates a quick overview of the candidate’s qualifications, experiences, skills, and achievements.
* Strengths: Identifies and highlights impactful elements of the resume.
* Weaknesses: Detects areas for improvement and offers customized suggestions.
* Job Title Suggestions: Recommends targeted job roles based on the resume’s content and user profile.

LinkedIn Data Scraping with Selenium:

* Through Selenium automation, users can input job titles and initiate a real-time scraping process on LinkedIn.
* Extracted data includes job titles, companies, locations, URLs, and detailed descriptions—giving users direct access to current opportunities.

