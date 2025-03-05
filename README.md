```markdown
# AI-powered Resume Screening and Ranking System

An interactive Streamlit web application that automates resume screening and ranking using a combination of classical NLP techniques and generative AI. The application extracts text from PDF resumes, processes the content using spaCy, computes quantitative similarity using TF-IDF and cosine similarity, and leverages Google’s Gemini-1.5 Pro model to provide qualitative suitability scores.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation and Setup](#installation-and-setup)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [License](#license)
- [Contact](#contact)

---

## Overview

Recruitment processes are often overwhelmed with high volumes of resumes, making manual screening time-consuming and error-prone. This project addresses the problem by:

- Extracting text from uploaded PDF resumes.
- Cleaning and processing the extracted text using spaCy.
- Computing resume-job description similarity using TF-IDF vectorization and cosine similarity.
- Integrating generative AI (Gemini-1.5 Pro) to generate qualitative suitability scores.
- Displaying ranked resumes in an intuitive Streamlit interface.

---

## Features

- **Drag-and-Drop Resume Upload:** Easily upload one or multiple PDF resumes.
- **Job Description Input:** Enter a job description for candidate matching.
- **Text Extraction & NLP Processing:** Automatic text extraction from PDFs and text normalization using spaCy.
- **Hybrid Ranking:** Combines quantitative analysis (TF-IDF) with qualitative insights from Gemini-1.5 Pro.
- **Interactive UI:** Built with Streamlit for a seamless user experience.
- **Environment Configuration:** Secure API key management via a `.env` file.

---

## Installation and Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/ai-resume-screening.git
   cd ai-resume-screening
   ```

2. **Create a Virtual Environment (Optional but Recommended):**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install Required Python Packages:**

   ```bash
   pip install -r requirements.txt
   ```

   If a `requirements.txt` file is not provided, install the packages manually:

   ```bash
   pip install streamlit spacy PyPDF2 scikit-learn google-generativeai python-dotenv
   ```

4. **Download the spaCy Model:**

   ```bash
   python -m spacy download en_core_web_sm
   ```

5. **Setup Environment Variables:**

   Create a `.env` file in the project root and add your Gemini API key:

   ```env
   GEMINI_API_KEY=your_actual_api_key_here
   ```

---

## Usage

1. **Run the Streamlit Application:**

   ```bash
   streamlit run app.py
   ```

2. **Using the Application:**
   - Enter the job description in the provided text area.
   - Drag and drop your PDF resume files into the uploader.
   - Click the **"Rank Resumes"** button to process and display ranked resumes with their respective suitability scores.

---

## Dependencies

- **Operating System:** Compatible with Windows, macOS, or Linux.
- **Programming Language:** Python 3.x
- **Development Environment:** Any IDE or code editor (e.g., VSCode, PyCharm)
- **Python Packages:** 
  - Streamlit
  - spaCy (with the `en_core_web_sm` model)
  - PyPDF2
  - scikit-learn
  - google-generativeai
  - python-dotenv
- **Other Software:** A web browser to access the Streamlit application.



