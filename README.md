# Web-API-And-Classification-Using-NLP-

1. Using Reddit website and Pushshift.io API, collecting posts from two subreddits of my choosing (r/basketball and r/football).
2. Use NLP to train a classifier model.

## Process followed:

1. Data collection done from Reddit using pushshift.io API
2. Data Cleaning and EDA(Exploratory Data Analysis)
3. Preprocessing and Modeling 
4. Comparison between various models
5. Conclusion

## Data Collection:

Pushshift was used for the data collection from the Community under Reddit website.
Data collected from pushshift was submissions from /r/Basketball and /r/football subreddits. 
After collecting the data, I analyzed submission posts for this projectin order to conduct a  comparison between these two subreddits.
In order to have a better understanding about the pushshift.io api , I checked the following video:
https://youtu.be/AcrjEWsMi

## Data Cleaning and EDA:

While cleaning the data, duplicates were dropped.Besides that , unnecessary data like  html, hyperlinks, punctuation, small words were cleared out. In addition to that , applied lemmatization and used stopwords to get rid of unwanted data. 

## Preprocessing and Modeling :

From scikit-learn, CountVectorizer and TfidfVectorizer were used to convert the text data to numeric features. TfidfVectorizer achieved a better accuracy score for a SVC model. Logistic regression, Random forest, and Multinomial naive Bayes models were tested with Gridsearch. Logistic regression performed the best using GridSearch technique.

## Conclusion:

Best scoring model: Multinomial Naive Bayes with Train / test scores: 0.8442 / 0.8481

Potential improvements:

Need to collect more data and indulge in more data cleaning and preprocessing of the given dataframe. 
Try to modify the stop words and filter out data like numbers and expressions. Practise more intensive gridsearch techniques using the parameters to optimize models.