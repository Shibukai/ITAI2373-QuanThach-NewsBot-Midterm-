# 🤖 NewsBot Intelligence System (ITAI 2373 Midterm)

## 📋 Project Overview
This project builds a fully automated, end-to-end Natural Language Processing (NLP) pipeline that transforms raw, unstructured news articles into an organized, queryable database layer. The underlying code automates data ingestion, string normalization, feature extraction, syntactic parsing, grammatical tagging, emotional tracking, and text classification.

* **Dataset Source:** [Kaggle Learn AI BBC News Dataset](https://www.kaggle.com/competitions/learn-ai-bbc/data)
* **Total Records:** 600 clean articles sampled evenly (120 per category) to optimize execution speed.
* **Core Categories:** Business, Entertainment, Politics, Sports, and Technology.

---

## 🙋‍♂️ Individual Project Contributions
Since I executed this project individually, I handled the entire design, debugging, feature engineering, and implementation of the system from scratch:

* **Ingestion & Automation (Module 1):** Swapped out the original blocking `files.upload()` prompt with an automated background configuration script (`os.environ['KAGGLE_API_TOKEN']`) to download and unzip the dataset on autopilot.
* **Text Preprocessing (Module 2):** Developed regex filters to clean HTML tags, URLs, emails, and punctuation before converting strings into dictionary base forms (lemmatization).
* **Feature Extraction (Modules 3 & 7):** Built a multi-class classification system using a TF-IDF vectorizer. Engineered an expanded feature matrix combining vocabulary scores with structural text counts and sentiment values, achieving a final **94.17% classification test accuracy**.
* **Linguistic & Syntax Analysis (Modules 4 & 5):** Managed NLTK part-of-speech tagging and spaCy dependency syntax mapping to track sentence structural complexity across different news fields.
* **Sentiment & Named Entities (Modules 6 & 8):** Deployed VADER sentiment tracking to evaluate text tones and applied spaCy to pull out 17,763 named entities, mapping them into an automatic relationship web.

---

## 🛠️ Repository Structure
```text
ITAI2373-NewsBot-Midterm/
│
├── learn-ai-bbc.zip                           # Reference document containing the original dataset URL
├── ITAI2372-QuanThach-Newbot-Midterm.ipynb    # Main Jupyter Notebook containing all Python code & plots
├── Newsbot_Reflections_QuanThach              # Journal
└── README.md                                  # Project documentation and individual reflections
```

---

## 🎥 Video Demonstration (Bonus Deliverable)
A comprehensive 5-7 minute video walking through the full code pipeline, live system inferences on new articles, dataset visualization outputs, and business value metrics has been recorded.

* **Video Demonstration Link:** [Insert your YouTube/Vimeo Link Here]
* **File Name Convention:** `MT_Video_Group_Solo_[Your_Full_Name]_ITAI2373`
