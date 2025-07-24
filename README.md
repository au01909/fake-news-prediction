Fake News Prediction

This project is a machine learning system to detect fake news articles using natural language processing and text classification techniques. Built in a Jupyter Notebook, it uses logistic regression on a labeled dataset of real and fake news.

Dataset

The dataset used is train.csv with the following columns:

- id: Unique identifier for each article
- title: Title of the news article
- author: Author of the article
- text: The main content (may be incomplete)
- label: Target variable (1 = Fake, 0 = Real)

Project Workflow

1. Data Preprocessing
   - Handling missing values
   - Combining title and author fields
   - Cleaning and stemming text using NLTK

2. Feature Extraction
   - Text is vectorized using TF-IDF (Term Frequency–Inverse Document Frequency)

3. Model Training
   - Dataset is split into training and test sets
   - Trained using Logistic Regression classifier

4. Evaluation
   - Model performance is evaluated using accuracy

5. Prediction System
   - Predicts whether a new/unseen news article is fake or real

Getting Started

1. Clone the repository

git clone https://github.com/au01909/fake-news-prediction.git
cd fake-news-prediction

2. Install dependencies

pip install numpy pandas nltk scikit-learn jupyter

3. Download NLTK resources

In a Python shell or notebook:

import nltk
nltk.download('stopwords')
nltk.download('punkt')

4. Launch the notebook

jupyter notebook Fake_News_Prediction.ipynb

Usage

- Run the notebook step by step
- Customize preprocessing or try other models
- Test with your own news headlines/articles in the prediction section

Results

- Logistic Regression gives strong performance
- Shows simple models with clean text features can flag fake news well

License

This project is licensed under the MIT License

Author

GitHub: https://github.com/au01909

