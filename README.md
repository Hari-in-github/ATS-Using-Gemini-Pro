# Application Tracking System Using Google's Gemini Pro

## Introduction
------------
The ATS Streamlit App is a Python application which works as an application tracking system, wherein it takes two inputs . One is job description and second is resume as a pdf document. And the ATS app provides a brief information related to resume and jb and how the resume matches with job description.


## How It Works
------------

![ATS Streamlit Application User Interface](./docs/Ats_Userinterface.png)

The application follows these steps to provide responses to your questions:

1. JOb Description : Takes input of the jd with which it has to compare the uploaded resume.

2. Resume uploading: The app reads the uploaded resume document and extracts its text content.

3. Language Model: The application utilizes a language model specifically Google's gemini pro to compare the resume with jd.

4. Response Generation: When you ask a question, The Jd and the text which is extracted from the resume are passed to the gemini pro model, then the user clicks either one of the two buttons , then the model compares the jd with the resume and either details of the resume or the percenatge match of the resume based on the option we choose will be displayed.


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
   a.Tell me about the resume 
   b.Percentage Match
   ```

## License
-------
The Apllication Tracking System App is released under the [MIT License](https://opensource.org/licenses/MIT).