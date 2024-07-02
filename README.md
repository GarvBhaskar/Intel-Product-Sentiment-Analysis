# Intel Products Sentiment Analysis Project

## Overview

Our primary objective was to build a web scraper to fetch Amazon product reviews for Intel products. The overall project involves scraping live review data, pre-processing and exploring this data, and applying various machine learning techniques to perform sentiment analysis and get insights on the performance of Intel processors.

## Team Details

- **Team Name:** Fractals
- **Members:** Aviral, Srivastava, Garv Bhaskar, Dinesh Kumar
- **Institution:** Vellore Institute of Technology, Chennai
- **Faculty Mentor:** Dr. Harini Sriraman

## Project Workflow

### Web Scraper Development
Developed a web scraper using Scrapy to extract product reviews from Amazon. The extracted review data is saved in a file named `data.csv` for further analysis.
- **GitHub Repo:** [Intel-Product-Sentiment-Analysis](#)
- **Model Script:** [model.py](#)

### Data Exploration and Preparation

#### Data Exploration
- Load data, plot distributions, generate word clouds, visualize common words.

#### Data Cleaning
- Remove HTML tags, punctuation, and stopwords; perform stemming and lemmatization.

### Feature Extraction
- **Bag of Words (BoW):** Transform text data into BoW and TF-IDF vectors.
- **Word2Vec:** Train Word2Vec models to create word embeddings.

### Model Building

#### Supervised Learning Models
- Naive Bayes (BernoulliNB, MultinomialNB)
- Logistic Regression
- Random Forest

#### Deep Learning Models
- LSTM (Long Short-Term Memory)
- Other RNNs (SimpleRNN, GRU)
- CNNs (Convolutional Neural Networks)

#### Embedding Layers
Utilize embedding layers in neural network models.

### Model Evaluation
Compare models and select the best-performing one.

### Visualization
Generate visual representations to illustrate key findings.

## Proposed Solution

Our solution integrates TF-IDF vectorization with Logistic Regression for baseline performance evaluation, leveraging Word2Vec embeddings initialized within an LSTM architecture for enhanced semantic understanding. We use NLTK for tokenization and cleaning, and TF-IDF for feature extraction. Logistic Regression is fine-tuned via GridSearchCV, and an LSTM model is trained in Keras with pretrained Word2Vec embeddings. Evaluation metrics include accuracy and visualizations like word clouds.

## Data Sources Used
Real-time reviews were collected from various e-commerce websites and social media platforms using web scraping tools like BeautifulSoup and Scrapy.

## Data Visualization
Plot the sentiment trends over time.

## Data Preparation
Focused on cleansing and tokenizing textual reviews, addressing punctuation and stop words, and converting reviews into numerical formats suitable for models like Bag of Words and Word2Vec.

## Data Exploration
Analyzed sentiment label distribution for balance, visualized brand-specific rating distributions, and examined statistical summaries of review lengths.

## Model Comparison
- **Benchmark Model:** CountVectorizer with Multinomial Naive Bayes
- **Other Models:** TfidfVectorizer with Logistic Regression, Pipeline and GridSearch

## LSTM with Word2Vec Embedding
1. Load pretrained word embedding model.
2. Construct embedding layer using embedding matrix as weights.
3. Train an LSTM with Word2Vec embedding (embedding layer => LSTM layer => dense layer).
4. Compile and fit the model using log loss function and ADAM optimizer.

## Word Clouds
<img src="image1.png" width="45%"> <img src="image2.png" width="45%">

## Summary Generation
Generated summaries to capture key insights from the sentiment analysis results.

## Images
<img src="image3.png" width="45%"> <img src="image4.png" width="45%">
