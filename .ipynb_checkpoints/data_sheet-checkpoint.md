# Datasheet 

There were two source of the information collected for this projects - both provided on Kaggle platform:
[1] CRM (Customer Relationship Management) Opportunities
https://www.kaggle.com/datasets/innocentmfa/crm-sales-opportunities?select=sales_pipeline.csv
[2] Consumer Reviews of Amazon Products
https://www.kaggle.com/datasets/datafiniti/consumer-reviews-of-amazon-products

## Motivation
[1] *CRM (Customer Relationship Management) Opportunities*
- For what purpose was the dataset created?
The dataset is designed to help data scientists and analytics understand the sales process, identify trends and patterns, and build predictive models to improve sales performance.
- Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?
Mursaleen Ameer (self-funded)

Both data sources then combined to create a synthetic data source for the model to be trained on.

[2] *Consumer Reviews of Amazon Products*
- For what purpose was the dataset created?
This dataset is a list of 5,000 consumer reviews for Amazon products like the Kindle, Fire TV Stick, and more from Datafiniti's Product Database updated between September 2017 and October 2018.
- Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?
Datafiniti (self-funded)
 
## Composition

- What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)?
  Both sources provide CSV files with textual and numerical data.
  
- How many instances of each type are there?
  Multiple CSV files.

  
- Is there any missing data?
  Given the model usees synthethic data-set there is nothing missed.

  
- Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by    doctor–patient confidentiality, data that includes the content of individuals’ non-public communications)?
  None

## Collection process

- How was the data acquired?

  Download from the Kaggle (kaggle.com)

- If the data is a sample of a larger subset, what was the sampling strategy?

  When synthetic data was build the sampling was done to match relative distribution of certain data points (see the notebook)
  
- Over what time frame was the data collected?

  Between September 2017 and October 2018

## Preprocessing/cleaning/labelling

- Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section.
  No pre-processing
  
- Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)?
  N/A
  
## Uses

- What other tasks could the dataset be used for?

  Optimizing sales team performance

- Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? For example, is there anything that a dataset consumer might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other risks or harms (e.g., legal risks, financial harms)? If so, please provide a description. Is there anything a dataset consumer could do to mitigate these risks or harms?

  None

- Are there tasks for which the dataset should not be used? If so, please provide a description.

  Dataset should not be used for sales person performance evaluation and related HR decisions.

## Distribution

- How has the dataset already been distributed?
  Uploaded to Github as part of the project.
  
- Is it subject to any copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?
  Yes first dataset is under CC BY-NC-SA 4.0(https://creativecommons.org/licenses/by-nc-sa/4.0/) licence, while the second is under Apache 2.0 (https://www.apache.org/licenses/LICENSE-2.0)
  
## Maintenance
- Who maintains the dataset?
  The synthetic dataset is maintained under this Github project. The original ones are maintained by Kaggle.