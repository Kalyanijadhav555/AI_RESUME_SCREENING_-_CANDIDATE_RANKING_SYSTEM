AI Resume Screening & Candidate Ranking System

Project Overview
The AI Resume Screening & Candidate Ranking System is an innovative solution designed to automate the resume screening process using Natural Language Processing (NLP). The system compares uploaded resumes with a given job description and generates a ranked list of candidates based on their relevance to the job. This significantly reduces manual effort, minimizes human bias, and ensures faster recruitment by instantly identifying the most suitable candidates.

The system uses TF-IDF (Term Frequency-Inverse Document Frequency) and Cosine Similarity to compare the textual content of resumes and job descriptions. It then outputs a ranked list with a matching score for each candidate, enabling recruiters to make data-driven hiring decisions.


Key Features
- Automated Resume Screening: Extracts and analyzes resume content.
- Candidate Ranking:  Ranks resumes based on similarity to the job description.
- Matching Score (%): Provides a percentage match score for each candidate.
- Streamlit Web Interface: Offers an interactive and easy-to-use UI.
- Bulk PDF Upload: Supports multiple resume uploads in PDF format.
- Bias-Free Screening: Ensures fair candidate shortlisting based on skills.



How It Works
1. Enter the Job Description: The recruiter enters the job description in the provided text area.
2. Upload Resumes:Upload one or more resumes in PDF format.
3. Resume Parsing: The system extracts text from the PDF files.
4. Similarity Matching: Using TF-IDF Vectorizer and Cosine Similarity, the system calculates the matching score.
5. Candidate Ranking: The output is a ranked list of candidates from highest to lowest match.


Technologies Used
| Technology        | Purpose                                  |
|-----------------|---------------------------------------------|
| Python          | Backend logic and processing              |
| Streamlit       | Frontend interface for the web app        |
| PyPDF2          | Extract text from PDF files                |
| Scikit-learn    | Implement TF-IDF and Cosine Similarity   |
| Pandas          | Data handling and structuring             |



Project Structure
The project directory contains the following files and folders:


AI-Resume-Screening/
│
├── app.py               # Main application file
├── requirements.txt     # Project dependencies
├── sample_resumes/      # Folder containing sample resumes
├── output/              # Stores generated output files
├── models/              # Model files (if applicable)
├── README.md            # Project documentation



Installation and Setup
Follow these steps to set up and run the project on your local system:

Step 1: Clone the Repository

git clone https://github.com/your-username/repository-name.git
cd repository-name

Step 2: Create a Virtual Environment (Optional)

python -m venv venv
source venv/bin/activate     # For MacOS/Linux
venv\Scripts\activate        # For Windows


Step 3: Install Dependencies

pip install -r requirements.txt


Step 4: Run the Application

streamlit run app.py

Step 5: Access the Application
Open your browser and go to:

http://localhost:8501


Expected Output
The system will generate a ranked list of candidates based on their resume content matching the job description. Example output:

| Resume Name                 | Matching Score (%) |
|-----------------------------|--------------------|
| Manjula_resume.pdf   | 39.48%             |
| Rasag_resume.pdf           | 35.46%             |
| NAGA_resume.pdf     | 29.24%             |
| Harsha_resume.pdf       | 28.76%             |
| Emma_watson.pdf              | 12.32%             |

The higher the matching score, the more suitable the candidate is for the job role.
