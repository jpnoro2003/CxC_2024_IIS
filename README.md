## CxC Data Hackathon 2024 - Infinite Investment Systems Challenge

## Inspiration
Everyday, Financial technology companies, or FinTechs, are constantly innovating to ensure that their products are the most appealing to customers. From financial planning to credit cards, there are many avenues for innovation within FinTech, especially leveraging Data Science and Machine Learning. For the Infinite Investment Systems Challenge, we were tasked with developing a machine learning model to predict customer churn for a growing investment platform. After predicting potentially churning customers, we were then tasked to devise a marketing strategy for the company to reduce their churn rate.
## What it does
We developed a pipeline that consumes the raw customer data, and through feature engineering techniques such as dummy value creation and text processing, outputs tabular data that can be leveraged by a machine learning model.
This data was then used to train a RandomForrestClassification Model that predicts whether a customer churns.
## How we built it
This model was built using Pandas, Numpy, datetime and sklearn. The preprocessing was done by using Pandas, NumPy and datetime to clean and reformat the raw data. Here, matplotlib was helpful in visualizing some of the features of the data.
Model development, training and tuning was done through Sklearn. A RandomForrestClassification Model was used.
## Challenges we ran into
While conducting exploratory analysis, we noticed that a lot of the entries in our dataset had missing fields, with some fields being almost completely empty across the dataset. If we trained our model using these fields, our model may become biased. We decided to remove columns which had over 70 percent of its values removed, as including these fields may harm the accuracy of our model. Upon further investigation, we discovered that a large subset of our training data had many columns null – we removed these columns as their data might be skewed by a system/reporting error.
## Accomplishments that we're proud of
Our model achieved an f1 score of 94.25% and a CV score of 93.22% on the filtered test data.

