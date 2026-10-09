# Career-Pilot
# 🚀 Career Pilot
### An AI-Powered Personalized Career Guidance and Placement Support System

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Enabled-green)
![Generative AI](https://img.shields.io/badge/Generative%20AI-LLM%20%7C%20RAG-purple)

## 📌 Overview

**Career Pilot** is an AI-powered career guidance and placement support platform designed for B.Tech students. It helps students identify suitable career paths, understand skill gaps, follow personalized learning roadmaps, practice Data Structures and Algorithms (DSA), and prepare for placements.

The platform integrates Machine Learning, Generative AI, recommendation techniques, and full-stack web development to provide career development resources in one place.

Career Pilot aims to answer three important questions:

- **What should I learn?**
- **Which skills do I need to improve?**
- **How can I prepare for my desired career?**

## 🎯 Problem Statement

B.Tech students often face difficulties in selecting suitable career paths, identifying missing skills, following structured learning roadmaps, and preparing effectively for placements. Learning resources, coding platforms, career guidance, and internship opportunities are frequently spread across different platforms.

Career Pilot aims to address these challenges through a centralized platform that provides personalized career recommendations, structured learning, skill-gap analysis, coding practice, placement preparation, and AI-based assistance.

## 🎯 Objectives

- Recommend suitable career domains based on student profiles, skills, and interests.
- Provide year-wise and domain-specific learning roadmaps.
- Identify missing skills and recommend learning activities.
- Support DSA practice and coding in multiple programming languages.
- Provide mock tests and placement preparation resources.
- Analyze student learning progress and placement readiness.
- Match students with relevant internships and hackathons.
- Provide an AI Assistant for career, technical, and programming queries.

## ✨ Key Features

### 1. AI-Based Career Recommendation
Uses a planned Random Forest classification model to recommend suitable career domains based on relevant student attributes.

Possible domains include:
- Data Science
- Data Analytics
- Artificial Intelligence and Machine Learning
- Web Development
- Cybersecurity
- Cloud Computing
- UI/UX Design

### 2. Personalized Learning Roadmaps
Provides structured learning paths based on a student's academic year, career goal, existing skills, and learning progress.

### 3. Skill-Gap Analysis
Compares the skills required for a selected career with the student's current skills and identifies areas that need improvement.

### 4. DSA and Coding Practice
Supports structured coding practice in:
- C
- C++
- Java
- Python
- JavaScript

The planned coding interface uses Monaco Editor, with Judge0 as a possible code execution service.

### 5. Mock Tests and Assessments
Provides assessment opportunities to help students evaluate their technical knowledge, DSA skills, and placement preparation.

### 6. Student Performance Clustering
Uses K-Means clustering to explore similarities between student skill and performance profiles and support personalized learning recommendations.

### 7. Placement Readiness
Analyzes available student performance indicators to highlight preparation strengths and areas for improvement.

### 8. Internship and Hackathon Opportunities
Collects opportunity information from permitted sources and matches opportunities with student profiles using criteria such as skills, academic year, domain, and eligibility.

### 9. AI Assistant
Uses Large Language Models (LLMs) to support:
- Career guidance
- Technical explanations
- Programming doubts
- DSA learning
- Interview preparation
- Resume and project guidance

### 10. Retrieval-Augmented Generation (RAG)
Retrieves relevant information from the Career Pilot knowledge base before generating answers, helping the AI Assistant provide context-aware responses.

### 11. Progress Dashboard
Helps students monitor roadmap completion, skills learned, mock-test performance, coding progress, and placement preparation.

## 🧠 AI and Machine Learning Components

| Component | Proposed Approach |
|---|---|
| Career recommendation | Random Forest |
| Student performance grouping | K-Means |
| Skill-gap analysis | Rule-based comparison |
| Learning resource recommendation | Content-based recommendation |
| Placement readiness | Analytical rules or a trained ML model, depending on available data |
| AI Assistant | Large Language Model |
| Knowledge retrieval | Retrieval-Augmented Generation (RAG) |
| AI workflow orchestration | LangChain |

**Note:** These are the intended approaches. Final algorithms and capabilities will depend on the implemented modules, available data, and evaluation results.

## 🏗️ System Architecture

```text
                 STUDENT
                    |
                    v
             React Frontend
                    |
                    v
              Flask REST API
                    |
          +---------+----------+
          |         |          |
          v         v          v
       MySQL      AI/ML     AI Assistant
      Database    Modules     LLM + RAG
                    |
          +---------+----------+
          |         |          |
          v         v          v
       Random     K-Means    Skill-Gap
       Forest                Analysis
          |
          v
    Career Recommendation
          |
          v
 Personalized Roadmap and
 Learning Recommendations
          |
          v
      Student Dashboard
```

## 🛠️ Technology Stack

### Frontend
- React.js
- JavaScript
- HTML5
- CSS3
- Tailwind CSS
- Chart.js
- Monaco Editor

### Backend
- Python
- Flask
- REST APIs

### Database
- MySQL

### Machine Learning and Data Processing
- Pandas
- NumPy
- Scikit-learn
- Joblib

### Generative AI
- Large Language Model API
- LangChain
- Retrieval-Augmented Generation (RAG)
- Vector database, such as ChromaDB

### Additional Integrations
- Judge0 for code execution
- APScheduler for scheduled opportunity collection
- Firebase Cloud Messaging (FCM) for push notifications

*Integrations listed above may be added as development progresses.*

## 📂 Project Structure

```text
CareerPilot/
│
├── frontend/                    # React frontend
│   └── src/
│       ├── components/
│       ├── pages/
│       ├── services/
│       ├── App.jsx
│       └── main.jsx
│
├── backend/                     # Flask backend
│   ├── app.py
│   ├── database.py
│   ├── routes/
│   ├── models/
│   └── services/
│
├── ai/                          # AI/ML modules
│   ├── data/
│   │   └── students.csv
│   ├── preprocessing/
│   │   └── preprocess.py
│   ├── career_model/
│   │   ├── train_model.py
│   │   └── predict.py
│   ├── clustering/
│   ├── skill_gap/
│   ├── placement/
│   ├── recommendation/
│   ├── chatbot/
│   ├── rag/
│   └── requirements.txt
│
├── database/
│   └── schema.sql
│
├── docs/
│
└── README.md
```

*Adjust this structure to match the files that actually exist in your repository.*

## ⚙️ Getting Started

### Prerequisites

Install the following tools:

- Python 3.12 or a compatible version
- Node.js and npm
- MySQL Server
- Visual Studio Code
- Git

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd CareerPilot
```

Replace the placeholder with your actual GitHub repository URL.

### 2. Set Up the AI/ML Environment

```bash
cd ai
python -m venv venv
```

Activate the environment on Windows:

```powershell
venv\Scripts\activate
```

Install the initial AI/ML dependencies:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn joblib
```

If a `requirements.txt` file is available, you can instead install the project's pinned dependencies with:

```bash
pip install -r requirements.txt
```

### 3. Prepare the Dataset

Place the student dataset at:

```text
ai/data/students.csv
```

The dataset should contain the features expected by the preprocessing and training scripts, along with a target column such as `career`.

Use properly labeled and documented data. If a sample dataset is synthetic, clearly identify it as synthetic.

### 4. Run Data Preprocessing

From the `ai` directory:

```bash
python preprocessing/preprocess.py
```

### 5. Train the Career Recommendation Model

Once the dataset and training script are ready:

```bash
python career_model/train_model.py
```

### 6. Run Career Prediction

After the model has been trained and saved:

```bash
python career_model/predict.py
```

These commands assume the files and relative paths match the project structure shown above.

### 7. Run the Frontend and Backend

Follow the setup instructions in the `frontend/` and `backend/` directories. Configure database credentials and any required API keys using environment variables. Do not commit secrets to GitHub.

## 📊 Model Evaluation

The machine learning modules should be evaluated using suitable metrics.

| Task | Evaluation |
|---|---|
| Career classification | Accuracy, Precision, Recall, F1-score, Confusion Matrix |
| Student clustering | Cluster characteristics and suitable clustering metrics |
| Placement classification | Accuracy, Precision, Recall, F1-score, if labeled data is available |
| Placement regression | MAE, RMSE, R², if predicting a numerical outcome |
| Recommendation | Relevance and usefulness of recommended resources |

Actual evaluation results should be reported only after running experiments on suitable data.

## 🔐 Privacy and Security

- Protect student profile information.
- Store credentials securely and never commit passwords or API keys.
- Validate user input at the backend.
- Use appropriate authentication and authorization.
- Use a sandboxed service for executing submitted code.
- Collect opportunity data only through permitted sources and methods.

## 🌱 Sustainable Development Goals

- **SDG 4 – Quality Education:** Supports accessible, structured, and personalized learning.
- **SDG 8 – Decent Work and Economic Growth:** Supports career preparation and employability.
- **SDG 9 – Industry, Innovation and Infrastructure:** Applies AI and software technologies to career development.

## 👥 Team Contributions

| Team Member | Responsibility |
|---|---|
| Person 1 | Frontend development, UI/UX, dashboard, and frontend integration |
| Person 2 | Backend development, MySQL database, REST APIs, opportunities, and notifications |
| Person 3 | AI/ML models, data preprocessing, skill-gap analysis, recommendations, LLM, and RAG |

## 🔮 Future Enhancements

- Improve career recommendations using larger, properly labeled datasets.
- Add adaptive roadmaps based on learning progress.
- Improve coding analytics and topic-wise recommendations.
- Expand internship and hackathon integrations.
- Add multilingual AI assistance.
- Evaluate recommendation quality through student feedback.
- Add explainable AI to help students understand career recommendations.

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a pull request.

## 📄 License

Choose a license before publishing the project for reuse. For example, an MIT License can be added by creating a `LICENSE` file containing the appropriate license text.

## 👩‍💻 Project Information

**Project Name:** Career Pilot  
**Project Type:** B.Tech Mini Project  
**Primary Domain:** Artificial Intelligence and Machine Learning  
**Application Domain:** Education Technology and Career Guidance

---

*Career Pilot aims to help students plan their careers, build relevant skills, and prepare systematically for industry opportunities.*
