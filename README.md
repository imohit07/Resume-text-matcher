# Resume-text-matcher
📄 Resume–Job Matching System using NLP
📌 Project Overview

This project automates the process of matching resumes with a given job description using Natural Language Processing (NLP) techniques. It helps identify the most relevant resume by measuring textual similarity between resumes and job requirements, reducing manual screening effort in recruitment processes.

The system uses TF-IDF vectorization and cosine similarity to rank resumes based on relevance.

🎯 Problem Statement

Recruiters often receive a large number of resumes for a single job role, making manual shortlisting time-consuming and subjective. Keyword-based filtering can miss good candidates due to wording differences.
This project aims to:

Automate resume screening

Rank resumes based on relevance

Reduce bias and manual effort

🛠️ Tech Stack

Python

Pandas – data handling

Scikit-learn

TF-IDF Vectorizer

Cosine Similarity

Regular Expressions (re) – text preprocessing

📂 Project Structure
├── UpdatedResumeDataSet.csv
├── resume_matching.ipynb
├── README.md

🔄 Workflow

Load resume dataset from CSV file

Accept a job description as input

Preprocess text (lowercasing, removing special characters)

Convert text into numerical vectors using TF-IDF

Compute cosine similarity between job description and resumes

Rank resumes based on similarity scores

Recommend the most relevant resume

🧠 Core NLP Logic
TF-IDF Vectorization

TF-IDF assigns importance to words based on:

How frequently a word appears in a document

How rare the word is across all documents

This ensures that important skills (e.g., Python, React) get higher weight than common words.

Cosine Similarity

Cosine similarity measures the angle between vectors, indicating how similar two documents are regardless of length.

cos
⁡
(
𝜃
)
=
𝐴
⋅
𝐵
∣
∣
𝐴
∣
∣
 
∣
∣
𝐵
∣
∣
cos(θ)=
∣∣A∣∣∣∣B∣∣
A⋅B
	​

📊 Output

Similarity score for each resume

Ranked list of resumes

Recommended resume with the highest relevance score

⚠️ Limitations

Relies on keyword similarity

Does not understand synonyms or context deeply

Experience level is not explicitly weighted

🚀 Future Enhancements

Use semantic embeddings (Word2Vec, GloVe, BERT)

Add experience and skill weighting

Support multiple job descriptions

Scale using vector databases for large datasets

📚 Learning Outcomes

Practical understanding of NLP preprocessing

TF-IDF and similarity-based ranking

Handling unstructured text data

Building explainable ML systems

📌 Disclaimer

This project is intended for educational and learning purposes only and should not be used as a standalone hiring decision system.
