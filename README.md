# YelpSentimentAnalysis
The goal of this project is to Perform sentiment classification on Yelp reviews dataset and Examine cross domain sentiment analysis on other platforms such as Amazon. 

## Summary
* Sentiment Analysis is a classification of the polarity of the given document into positive, negative or neutral. 
## Why sentiment analysis is important in social media and analytics?
* Sentiment analysis can be an excellent source of information for both customers, business owners and can provide insights that can:
	* Determine marketing strategy
	* Improve campaign success
	* Improve customer service
	* Evaluating the brand's health
	* Help customer to make purchase decisions

* People use Yelp to find good restaurants and other business services. Yelp provides a platform to customers to rate businesses by giving star ratings and writing reviews.

* This study performs sentiment analyis on the "Yelp review dataset" which is available on Kaggle.

## Experiment 1: Does transforming the "term frequency" matrix of our reviews into "tf-idf" scores improve the performance of our models?  

* Used "Bag of words" approach which uses "term frequency" as a feature. Logistic Regression and Multinomial Naive Bayes models are used to decipher the sentiment tendency of each review.
*Performance is compared with using the "tf-idf" (term frequency - inverse document frequency) as a relative feature. 

## Experiment 2: Does using dictionaries of positive and negative words bring performance gains? 

* Trained the model using dictionary of positive and negative words as an additional predictor variable to the "text" of the reviews. Compared the performance using Logistic Regression and Multinomial Naive Bayes models. 
* Found out the distribution of different star ratings correctly classified or incorrectly classified into positive or negative class. 

## Experiment 3: Can we transfer learning of sentiments from one domain to another? 

* Inspiration: Generating labelled training data is expensive and time consuming. What if we can use already existing dataset from another  domain? 
* In-domain is defined as the domain "where the learning is transfered to"
* Out-domain is defined as the domain "where the learning is transfered from"

### 3a.: In-domain - Yelp reviews dataset, Out-domain - Amazon reviews dataset. 
* Method 1: Train the model using Amazon reviews dataset and report model performance on the held out test set (sampled from Yelp reviews dataset). 
* Method 2: Train the model on the combined Amazon and the Yelp dataset (excluding the test set) and and report model performance on the held out test set.

### 3b: In-domain - Amazon reviews dataset, Out-domain - Yelp reviews dataset. 
* Method 1: Train the model using Yelp reviews dataset and report model performance on the held out test set (sampled from Amazon reviews dataset). 
* Method 2: Train the model on the combined Yelp dataset and Amazon dataset (excluding the test set) and and report model performance on the held out test set.

