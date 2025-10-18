# Model Card

I used two models to build recommendaiton -  tabularisai/multilingual-sentiment-analysis and decision tree.

Model Name: tabularisai/multilingual-sentiment-analysis
Base Model: distilbert/distilbert-base-multilingual-cased
Task: Text Classification (Sentiment Analysis)
Languages: Supports English plus Chinese (中文), Spanish (Español), Hindi (हिन्दी), Arabic (العربية), Bengali (বাংলা), Portuguese (Português), Russian (Русский), Japanese (日本語), German (Deutsch), Malay (Bahasa Melayu), Telugu (తెలుగు), Vietnamese (Tiếng Việt), Korean (한국어), French (Français), Turkish (Türkçe), Italian (Italiano), Polish (Polski), Ukrainian (Українська), Tagalog, Dutch (Nederlands), Swiss German (Schweizerdeutsch), and Swahili.
Number of Classes: 5 (Very Negative, Negative, Neutral, Positive, Very Positive)

## Model Description

**Input:** Client accounts data and sentiment of the client's feedback for the product.

**Output:** Rank of the opporutnity

**Model Architecture:** 

## Performance

Give a summary graph or metrics of how the model performs. Remember to include how you are measuring the performance and what data you analysed it on. 

## Limitations

Outline the limitations of your model.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
