Fake News Detection using Machine Learning

📌 Project Overview
-This project implements an end-to-end Fake News Detection system using Natural Language Processing (NLP) and Machine Learning techniques. The goal is to classify news articles as Fake or Real based on their textual content.
-Two feature extraction methods — Bag of Words (BoW) and TF-IDF — are compared using a Random Forest classifier.

📊 Dataset
The project uses the Fake and Real News Dataset from Kaggle.
-Fake.csv – Fake news articles
-True.csv – Real news articles
Due to GitHub file size limits, the dataset is not included in the repository. It can be downloaded directly from Kaggle using the provided code in the notebook.

Each article contains:
-Title
-Text
-Subject
-Date
A binary label is created:
-1 → Fake News
-0 → Real News
-Only the text column is used for model training.

⚙️ Project Workflow
1. Dataset loading and labeling
2. Data cleaning and preprocessing
3. Exploratory Data Analysis (EDA)
4. Text preprocessing (stopword removal, lemmatization)
5. Feature extraction using BoW and TF-IDF
6. Model training using Random Forest
7. Model evaluation and visualization
8. Feature importance analysis
9. Saving the trained model and vectorizer

🧠 Text Preprocessing
-Lowercasing
-Removal of special characters and numbers
-Custom stopword removal (negative words retained)
-Lemmatization
This ensures meaningful text representation while preserving important semantic information.

🏗️ Models Used
-Random Forest Classifier
--Bag of Words features
--TF-IDF features

📈 Model Performance
Model	Accuracy
Bag of Words + Random Forest	99.66%
TF-IDF + Random Forest	99.65%
Both models performed exceptionally well, with Bag-of-Words achieving slightly higher accuracy.

📊 Visualizations Included
-Class distribution plot
-Confusion matrix
-Feature importance plot
These visualizations help in understanding data characteristics and model behavior.

💾 Model Saving
The trained TF-IDF vectorizer and Random Forest model are saved using joblib for future reuse and deployment.

🛠️ Technologies Used
-Python
-Pandas, NumPy
-NLTK
-Scikit-learn
-Matplotlib, Seaborn

✅ Conclusion
This project demonstrates a complete NLP pipeline for fake news detection using classical machine learning techniques. It highlights the importance of proper preprocessing, feature extraction, and evaluation in building reliable text classification systems.
