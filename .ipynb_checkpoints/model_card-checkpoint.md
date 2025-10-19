# Model Card

We have used multiple models to build ensemble:

[1] tabularisai/multilingual-sentiment-analysis

Model Name: tabularisai/multilingual-sentiment-analysis
Base Model: distilbert/distilbert-base-multilingual-cased
Task: Text Classification (Sentiment Analysis)
Languages: Supports English plus Chinese (中文), Spanish (Español), Hindi (हिन्दी), Arabic (العربية), Bengali (বাংলা), Portuguese (Português), Russian (Русский), Japanese (日本語), German (Deutsch), Malay (Bahasa Melayu), Telugu (తెలుగు), Vietnamese (Tiếng Việt), Korean (한국어), French (Français), Turkish (Türkçe), Italian (Italiano), Polish (Polski), Ukrainian (Українська), Tagalog, Dutch (Nederlands), Swiss German (Schweizerdeutsch), and Swahili.
Number of Classes: 5 (Very Negative, Negative, Neutral, Positive, Very Positive)

[2] GradientBoostingClassifier from SkLearn - see https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingClassifier.html
[3] RandomForest Classisfier - see https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
[4] Logistic Regression

## Model Description

**Input:** Client accounts data and sentiment of the client's feedback for the product.

**Output:** Probability of the win and loss for a given opportunity 

**Model Architecture:** 
1. Data is enhanced with sentiment analysis for the clietn feedback
2. An ensemble model applied with GradientBoosting and RandomForest classifiers used as a base, while Logistic regression used as a metamodel.


## Performance

**Meta-model weights (higher -> more influence):**
Intercept: 1.026676149653994
RandomForest_proba    0.228467
GradientBoost_proba   -0.999474

**The model shows stable predictive power:**
Train success rate 63.15% 
Validation: 63.14%

## Limitations

Model has been trained on very small sample.

## Trade-offs

Input data in terms of the product reviews showed strong positive bias - further test and training on a more diverse client feedback.