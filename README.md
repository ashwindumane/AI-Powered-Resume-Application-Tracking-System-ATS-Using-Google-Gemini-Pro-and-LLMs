# AI-Powered-Resume-Application-Tracking-System-ATS-Using-Google-Gemini-Pro-and-LLMs 🚀💥
Designed and implemented an AI-powered Resume Application Tracking System(ATS) leveraging Google Gemini Pro and advanced LLMs to streamline recruitment processes. The system automates resume parsing, skill matching, and job recommendations with high accuracy and efficiency.

## Problem Statement: 
Many resumes are rejected by Applicant Tracking Systems (ATS) due to keyword mismatches and formatting issues.

## Solution: 
Our AI-powered Resume ATS helps you optimize your resume for maximum impact & improving your chances of getting noticed by recruiters.Elevate Your Job Search With our AI-powered ATS(Application Tracking System), you can increase your chances of getting noticed by recruiters and landing your dream job 🚀💥

## Key Features:

**1.Intelligent Resume Analysis:**
Extracts key information from your resume.
Identifies missing keywords and suggests improvements.
Compares your resume to job descriptions for a better match.

**2.Personalized Feedback:**
Receives tailored advice on how to enhance your resume's effectiveness.
Identifies strengths and weaknesses in your resume.

**3.User-Friendly Interface:**
Easy-to-use platform with a clear and intuitive design.
Upload your resume and job description for quick analysis.

## How It Works:

**1.Upload Your Resume:**
Simply upload your resume in PDF format.
**2.Enter Job Description:**
Paste the job description you're targeting.
**3.Get Instant Insights:**
Receive a detailed analysis of your resume, including:
Match score with the job description.
Missing keywords to add.
Suggestions for improvement.

## Architectural Diagram : 
![architectural diagram](https://github.com/user-attachments/assets/fa04a229-68f0-4065-80d6-f6d46892a646)

## Applicant Tracking System : 
![Applicant Tracking System](https://github.com/user-attachments/assets/49678cf9-1610-474c-983f-6e1a6edb19c4)

## Tools and Libraries 🚀💥
- **Code Editor:** Visual Studio Code
- **Language:** Python
- **Frontend:** Streamlit (Python Web Framework)
- **Hosting:** GitHub
- **LLM API:** Google Gemini Pro

## Steps to Create the Project

### 1. Environment Setup
- Create a Python environment:
  ```bash
  conda create -p atsenv python==3.10 -y
  ```
- Activate the environment:
  ```bash
  conda activate atsenv/
  ```

### 2. Install Dependencies
- Create a `requirements.txt` file to list the necessary libraries and frameworks.
- Add the required dependencies and install them:
  ```bash
  pip install -r requirements.txt
  ```

### 3. Secure API Key with .env File
- Go to your browser and search for **Makersuite**.
- Sign up and create an API key.
- Create a `.env` file in your project folder and add the following:
  ```plaintext
  GOOGLE_API_KEY='YOUR_API_KEY'
  ```

### 4. Workflow of the Application
1. **Setup Poppler:** Ensure Poppler is installed for PDF processing.
2. **API Integration:** Integrate the Google Gemini Pro API.
3. **PDF to Text:** Use `pypdf` to extract text from resumes.
4. **Pass Text to API:** Send the extracted text to the LLM API and retrieve responses.

### 5. Develop the Application
- Create an `app.py` file for the application code.
- Code structure:
  1. **Import Requirements:** Import necessary libraries and modules.
  2. **API Response Function:**
     ```python
     def get_gemini_response(input_text):
         # Function to send text to the Gemini API and retrieve a response
     ```
  3. **PDF Text Extraction Function:**
     ```python
     def input_pdf_text(pdf_path):
         # Function to extract text from a given PDF file
     ```
  4. **Prompt Template:** Create a variable for the prompt template.
  5. **Streamlit App:** Develop the main Streamlit app functionality.

### 6. Run the Application
- Open the terminal and navigate to the project folder containing `app.py`.
- Start the application:
  ```bash
  streamlit run app.py
  ```
- Open the provided URL in your browser:
  ```plaintext
  Local URL: http://localhost:8501
