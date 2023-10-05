# SMS Sentiment Analysis

## Analyzing SMS Messages for Sentiment Insights

*A case study by Waqas Ahmad*

## 1. Introduction

This project focuses on performing comprehensive sentiment analysis on a dataset containing SMS chat messages. The primary objective is to create a model that accurately classifies text messages and to gain insights into the sentiment present in the messages. Additionally, we aim to compare the general sentiment of messages across different countries, exploring patterns and variations in communication styles.

## 2. Language and Libraries

The project is implemented using the Python programming language, leveraging various libraries for data analysis and natural language processing (NLP). The key libraries used include:

- **Python**: The primary programming language for data analysis and processing.
- **Pandas**: Utilized for data manipulation, exploration, and structuring.
- **NLTK (Natural Language Toolkit)**: Applied for advanced NLP tasks such as tokenization and sentiment analysis.
- **Matplotlib and Seaborn**: Used for data visualization to present insights effectively.

## 3. Dataset

The dataset employed in this project is derived from a CSV file named `clean_nus_sms.csv`. This dataset comprises SMS chat data and encompasses several important columns:

- **id**: A unique identifier for each message.
- **Message**: The actual text content of the SMS messages.
- **length**: The character length of each message.
- **country**: The country or origin of the sender.
- **Date**: The date on which each message was sent.

## 4. Stages

1. **Data Import & Overview**
2. **Planning Analysis**
3. **Choosing NLP Model/Technique**
4. **Text Preprocessing**
5. **Analysis**
   - Exploratory Data Analysis
   - Sentiment Analysis
   - Feature Selection for classifier
6. **Data Splitting**
7. **Model Selection**
   - Message Classification/Model Evaluation
8. **Sentiment Distribution & Analysis by Country**
9. **Conclusion & Insights**
10. **Future Directions**

## 5. Data Preprocessing

### 5.1. Data Import and Overview

The initial step involves importing the dataset using Pandas and obtaining a holistic understanding of the data structure through functions like `.head()` and `.info()`.

### 5.2. Text Preprocessing

Text preprocessing is pivotal to ensure the reliability of sentiment analysis. Key preprocessing steps include:

- Eliminating empty messages: Rows with missing or empty messages are removed.
- Text normalization: All text is converted to lowercase to ensure consistent analysis.
- Punctuation removal: Punctuation marks are stripped from the text.
- Tokenization: The text is split into individual words or tokens.
- URL and HTML tag removal: Any URLs and HTML tags are removed from the messages.

## 6. Sentiment Analysis

### 6.1. Sentiment Model

A Naive Bayes classifier from the NLTK library is employed for sentiment analysis. To train this model, a labeled dataset containing positive and negative sentiments is used as a reference. The classifier learns from this data to make predictions on the sentiment of SMS messages.

### 6.2. Model Evaluation

The Naive Bayes classifier exhibits impressive performance, achieving an accuracy rate of approximately 99.63% on the test set. Additionally, the model identifies the most informative features for sentiment prediction, aiding in interpreting its decision-making process.

### 6.3. Sentiment Classification

With the trained model, sentiment classification is applied to each message within the dataset. Messages are categorized as either positive or negative based on their sentiment scores.

## 7. Exploratory Data Analysis

Exploratory Data Analysis (EDA) is an integral part of the project, helping to uncover underlying patterns and trends in the dataset. Key aspects of the EDA include:

- Distribution of Messages by Country: Visualizations showcase the number of messages sent from each country, highlighting the most active countries.
- Sentiment Distribution: Visualization and analysis of the distribution of sentiment in the dataset, including the proportion of positive and negative messages.

## 8. Results and Insights

### 8.1. Sentiment Distribution

An analysis of the sentiment distribution reveals that approximately 64.3% of the messages are classified as negative, while around 35.8% are classified as positive. This suggests a prevalence of negative sentiment in the SMS messages.

### 8.2. Sentiment Analysis by Country

The sentiment analysis is further dissected by country to determine which countries exhibit a higher proportion of positive or negative messages. Key insights include:

- Trinidad and Tobago: This country has the highest proportion of positive messages.
- Barbados: Barbados has the highest proportion of negative messages.

These findings provide valuable insights into the sentiment expressed in SMS communication across different regions.

## 9. Conclusion and Future Directions

Using a sentiment classification model, I evaluated the sentiments of messages within the NUS SMS Corpus. The model classified messages as either positive or negative, providing insights into the overall sentiment distribution. this project successfully conducts sentiment analysis on SMS chat data, offering valuable insights into the sentiment patterns within the dataset. The Naive Bayes classifier demonstrates remarkable accuracy, but further model enhancements and evaluations are recommended for robust generalization to new data. 

### Insights:

- The sentiment analysis revealed that approximately 64.3% of the messages in the NUS SMS Corpus were classified as negative, while about 35.8% were classified as positive.
- When comparing sentiment by country, Trinidad and Tobago, Nepal, and Morocco exhibited the highest positivity scores, while Lebanon, Barbados, and Nigeria displayed the highest negativity scores in the sentiment analysis.
- Trinidad and Tobago had the highest positivity, while Lebanon showed the highest negativity in the sentiment analysis, as illustrated in the graph.

This analysis helps us understand the prevailing sentiment patterns in the SMS communication dataset, highlighting countries with varying degrees of positivity and negativity in their messages.

Future directions for this project may include:

- Evaluating and implementing more advanced sentiment analysis models.
- Hyperparameter tuning to optimize model performance.
- Analyzing the impact of sentiment on specific date ranges or events.
- Exploring potential correlations between sentiment and message length.
- Enhanced Sentiment Analysis: Explore advanced sentiment models to further improve accuracy and classification.
- Hyperparameter Optimization: Fine-tune model parameters for better performance.
- Temporal Analysis: Investigate sentiment changes over time and in response to events.
- Message Length Correlation: Analyze how message length relates to sentiment.
- Multilingual Support: Extend analysis to multiple languages if applicable.
- Real-time Sentiment: Develop real-time analysis for applications like customer service.
- Interactive Visualization: Create user-friendly sentiment trend dashboards.
- Emotion Analysis: Explore a wider range of emotions beyond positive and negative.
- User Profiling: Investigate how demographics affect communication patterns.
- Data Expansion: Collect additional SMS data from diverse sources and periods.

These future steps will enhance the project's capabilities and provide deeper insights into SMS communication patterns.
Overall, this project serves as a foundational analysis of SMS chat data, offering valuable insights into communication patterns and sentiment expressions across different countries.
