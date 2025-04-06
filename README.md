# resume-analyzer
 Resume Classification using NLP & Logistic Regression
This project focuses on classifying resumes into various job categories using Natural Language Processing (NLP) techniques and a Logistic Regression model. The goal is to automate resume screening by identifying the category of a resume, such as Data Science, HR, Sales, etc.

📦 Libraries Used
pandas
numpy – Data manipulation
matplotlib, seaborn – Visualization

nltk – Text preprocessing and tokenization

re, string – Regex and punctuation handling

wordcloud – Word cloud visualization

sklearn – Machine learning model and evaluation

📁 Dataset
Name: UpdatedResumeDataSet.csv

Columns:

Category: The category of the resume (e.g., Data Science, HR, etc.)

Resume: The text of the resume

🔍 Steps Performed
1. Exploratory Data Analysis (EDA)
Checked data info and missing values

Visualized resume distribution by category

Analyzed word count distribution in resumes

2. Data Cleaning
Removed URLs, special characters, mentions, hashtags, etc.

Applied custom cleaning function to preprocess resume text

3. Text Processing
Tokenized cleaned resume text

Removed stopwords

Created frequency distribution of top words

Generated a Word Cloud for visualization

4. Feature Engineering
Used TF-IDF Vectorizer to convert text into numerical features

Limited features to the top 1000 for efficiency

5. Model Building
Applied Label Encoding to categories

Split dataset into training and testing sets

Trained a Logistic Regression model

6. Evaluation
Evaluated model performance using Accuracy Score and Classification Report

📊 Results
Model: Logistic Regression

Accuracy: Achieved on test data

Output: Printed Classification Report with precision, recall, and F1-score

📌 How to Run
Install required libraries:

bash
Copy
Edit
pip install pandas numpy matplotlib seaborn nltk scikit-learn wordcloud
Download NLTK stopwords and tokenizer:

python
Copy
Edit
import nltk
nltk.download('punkt')
nltk.download('stopwords')
Load the dataset and run the Python script (or Jupyter Notebook).

📈 Sample Visualizations
Resume Category Distribution (Bar Chart)

Word Count Histogram

Top 50 Frequent Words (Text Output)

Word Cloud

🤔 Future Improvements
Use advanced models like SVM, Random Forest, or Neural Networks

Fine-tune preprocessing pipeline

Add resume parsing for structured input

Deploy model using Flask or Streamlit

👨‍💻 Author
Built with ❤️ using Python and scikit-learn

