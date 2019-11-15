# ABSA
## Aspect Based Sentiment Analysis

Retrieves aspects from the user reviews with sentiment score.

** Aspects: {Value, Food, Drinks, Staff, Service, Ambience, Location and Price}

## Datasources Extraction:
Training Datasources: (Fetch data from) 
** Google places API - 
•	https://maps.googleapis.com/maps/api/place/nearbysearch/json
•	https://maps.googleapis.com/maps/api/place/details/json
** Zomato API - 
•	https://developers.zomato.com/api/v2.1/locations,
•	https://developers.zomato.com/api/v2.1/location_details,
•	https://developers.zomato.com/api/v2.1/reviews)
** Twitter
•	tweepy.OAuthHandler
•	tweepy.API
•	tweepy.Cursor
** CitySearch scraping
•	http://www.citysearch.com/listings/houston-tx-metro/restaurants.html

## Test Data of: (Manually fetch and test)
** TripAdvisor 
•	from Kaggle, for testing

## Data Preparation:
* Data cleaning (emojis, date formats, text formats)
* XML formatting of Review and each aspect in it.

## Steps for Training:
* Pretrained BERT
* Parse and pass XML for training.
* Vectorization using SpaCy.
* 4 fold Cross validation

## Model Preparation:
* Aspects extraction 
* MultinomialNaiveBayes
* Sentiment Score

## Testing Accuracy:
* Confusion matrix
* Multiclass classification
