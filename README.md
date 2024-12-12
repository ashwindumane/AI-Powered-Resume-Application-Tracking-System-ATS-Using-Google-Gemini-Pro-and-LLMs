# AI-Powered-Resume-Application-Tracking-System-ATS-Using-Google-Gemini-Pro-and-LLMs
Designed and implemented an AI-powered Resume Application Tracking System(ATS) leveraging Google Gemini Pro and advanced LLMs to streamline recruitment processes. The system automates resume parsing, skill matching, and job recommendations with high accuracy and efficiency.

# Architectural Diagram : 
![architectural diagram](https://github.com/user-attachments/assets/fa04a229-68f0-4065-80d6-f6d46892a646)

# Applicant Tracking System : 
![Applicant Tracking System](https://github.com/user-attachments/assets/49678cf9-1610-474c-983f-6e1a6edb19c4)


### Use tools and Libraries
 - Code Editor --> Visual Studio Code Editor
 - Language --> python
 - frontend --> streamlit(python web Framework)
 - Host --> github
 - LLm API  --> Google gemini pro 
--------------
# STEPS to create Project
1. Environment setup
    - `conda create -p atsenv python==3.10 -y`
    - Activate environemt `conda activate atsenv/`
      
2. Create the requirements.txt to install important libraries and framework
    - IN requirements.txt add important libraries and framework
    - Save and run CMD `pip install -r requeriment.txt` 

3. create .env file in project folder to save the api key secure
    - Go to browser and search "Makersuite"
    - signup and click on create API key  
    - copy the api key and paste in .env file
    - `GOOGLE_API_KEY = 'YOUR_API_KEY'`
      
4. Deacribe the workFlow of website
    - setup poppler 
    - api integrate
    - pdf to text --> pypdf
    - text pass to API and return response
    - 
4. Create the app.py to develop application code
    - Import all requirements
    - Create get_gemini_response function to get the model and pass the input
    - Create the input_pdf_text fuction to extract text from pdf
    - Create a prompt_input variable  where pass the prompt template of response
    - Create a Basic streamlit app functionality in app

5. RUN THE APP 
    - Open to CMD 
    - Go to the project folder where the app.py 
    - run `streamlit run app.py`
    - then go to browser paste `Local URL: http://localhost:8501`

# End-to-End AI-Powered Resume Application Tracking System

This repository hosts the code and resources for building an AI-powered Resume Application Tracking System leveraging Google Gemini Pro and Streamlit. The application is designed to extract, analyze, and evaluate resumes efficiently using cutting-edge technologies.

## Tools and Libraries
- **Code Editor:** Visual Studio Code
- **Language:** Python
- **Frontend:** Streamlit (Python Web Framework)
- **Hosting:** GitHub
- **LLM API:** Google Gemini Pro

---

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
  


