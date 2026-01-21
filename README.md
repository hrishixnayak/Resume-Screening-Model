📄 Jinino Resume Screening System (ML + Streamlit)

An end-to-end Machine Learning–based Resume Screening System built to help Jinino automatically evaluate candidate resumes and decide whether they are a good fit for the company.

The system accepts real PDF resumes, processes them using NLP techniques, and outputs a Fit / Not Fit decision with a confidence score.

🚀 Features

📄 Upload PDF resumes

🧹 Text cleaning & preprocessing

🧠 ML-based resume evaluation

📊 Fit score using probability

✅ Clear decision: Fit for Jinino / Not a Fit

🌐 Simple web interface using Streamlit

🧠 How It Works

A resume PDF is uploaded through the web app

Text is extracted from the PDF

The text is cleaned and normalized

A trained TF-IDF vectorizer converts text into numerical features

A trained Machine Learning model predicts:

Fit probability

Final decision based on threshold

🛠️ Tech Stack

Python

Scikit-learn

Natural Language Processing (NLP)

TF-IDF Vectorization

Streamlit (Web UI)

PyPDF2 (PDF text extraction)

Pickle (Model persistence)

📂 Project Structure
jinino_resume_app/
│
├── app.py              # Streamlit web application
├── model.pkl           # Trained ML model
├── vectorizer.pkl      # Trained TF-IDF vectorizer
├── README.md           # Project documentation

⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/your-username/jinino-resume-screening.git
cd jinino-resume-screening

2️⃣ Install dependencies
pip install -r requirements.txt


If requirements.txt is not present:

pip install streamlit scikit-learn PyPDF2

▶️ Run the Application
streamlit run app.py


The app will open at:

http://localhost:8501

🧪 Usage

Open the web app in your browser

Upload a resume PDF

Click Predict Fit

View:

Fit score

Decision: ✅ Fit for Jinino / ❌ Not a Fit

📊 Decision Logic
Fit Score	Decision
≥ 0.75	✅ Fit for Jinino
< 0.75	❌ Not a Fit

(Threshold can be adjusted based on hiring needs)

🎯 Use Cases

Resume shortlisting for startups

Early-stage ATS prototype

Learning project for ML + NLP + deployment

Internal hiring tool for Jinino

🔮 Future Improvements

Skill-level explanation (“why this resume is a fit”)

Multiple job role support

Resume ranking system

Database storage of results

Cloud deployment (Streamlit Cloud / AWS)

👤 Author

Hrishikesh Nayak
Machine Learning & Data Analytics Enthusiast
Built as part of a real-world ML project for Jinino

⭐ Acknowledgements

Kaggle (dataset inspiration)

Scikit-learn & Streamlit communities
