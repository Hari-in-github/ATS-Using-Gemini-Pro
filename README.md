# Application Tracking System Using Google's Gemini Pro

## Introduction
------------
The ATS Streamlit Application integrates Google's Gemini Pro model to streamline resume evaluation. Users input job descriptions and upload resumes in PDF format, receiving detailed insights or percentage matches. With an intuitive interface, it enhances recruitment processes by efficiently analyzing candidate profiles and aligning them with specified job requirements.


## How It Works
------------

![ATS Streamlit Application User Interface](./docs/Ats_Userinterface.png)

1. Job Description Input:

   User provides the Job Description (jd) as input to the application.
   This Job Description serves as the benchmark against which uploaded resumes will be evaluated.

2. Resume Uploading:
   
   User uploads a resume document in PDF format.
   The application reads the uploaded PDF resume and extracts its text content for further processing.

3. Language Model Configuration:

   The application is configured to use Google's Gemini Pro language model for natural language processing tasks.

4. Response Generation:

   User initiates the question/response process by clicking on one of the buttons:
   "Tell Me About the Resume" or
   "Percentage Match."
   The extracted resume text and the provided Job Description are passed to the Gemini Pro model for analysis.
   For "Tell Me About the Resume" Button:

   The application requests the Gemini Pro model to generate detailed information about the alignment of the resume with the Job Description.
   Gemini Pro processes the input and provides a response highlighting strengths and weaknesses, evaluating how well the candidate's profile aligns with the specified job requirements.

   For "Percentage Match" Button:

   The application requests the Gemini Pro model to calculate the percentage match between the resume and the provided Job Description.
   Gemini Pro performs the comparison and provides the percentage match as output.
   Additionally, the application may display keywords missing in the resume and final thoughts on the match.
   The generated response is presented to the user.


## Dependencies and Installation
----------------------------
To install the Application Tracking System App, please follow these steps:

1. Clone the repository to your local machine.

2. Install the required dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

3. Obtain an Google API key from Google's marksuite website and add it to the `.env` file in the project directory.
```commandline
OPENAI_API_KEY=your_secrit_api_key
```

## Usage
-----
To use ATS Streamlit App, follow these steps:

1. Ensure that you have installed the required dependencies and added the Google API key to the `.env` file.

2. Run the `main.py` file using the Streamlit CLI. Execute the following command:
   ```
   streamlit run app.py
   ```

3. The application will launch in your default web browser, displaying the user interface.

4. Input the job description and add resume as a PDF document into the app by following the provided instructions.

5. Click either one of two buttons displayed.
   ```
   a. Tell me about the resume 
   b. Percentage Match
   ```

## License
-------
The Apllication Tracking System App is released under the [MIT License](https://opensource.org/licenses/MIT).