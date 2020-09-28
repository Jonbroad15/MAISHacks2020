# Scam Product Detector
## Research Questions
- In light of the increased usage of online webpages to purchase products, you aren't sure are just sometimes which are legitimate products are something that was made to have been given 5 stars from bot rating accounts.
- Is it possible to train a model to predict whether a product crosses a given legitimacy threshold. 

## Prediction Methods
- The validation data required to compute a supervised learning model is a feature which could possibly annotated?
- Can possibly start with an unsupervised model. Feature weights will give an idea of what constitutes a legitimate product.
- Or possible to instead construct an algorithm that predicts bot reviews 
- Translate reviews to English test
  - Deepl.com
	- Google translate api/plugin

## Data Collection
- Download all reviews for a given set of products
- Use amazon certified products as a positive validation set
- Negative validation set 
  ○ Certified scam list
  ○ Sketchy websites
    § Ebay
    § Craigslist
    § Amazon may have some too

## Data Annotation
### Native features:
  - Start rating distribution (mean, CI, variance)
  - Number of reviews
  - Avg. review length
### Generated Features
- Proportion of review from bots
- Need a model to predict which reviews are bots
- Adjusted non-bot star rating, num of reviews, avg review length
  - Occurrences of words from scam dictionary
    - i.e. {'fake', 'scam', '…' }

## Techniques
- Natural Language processing
  ○ API?
  ○ Python package?
    § NLTK

## Applications/UI
- Chrome extension

