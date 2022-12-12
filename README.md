# Natural-Language-Processing-Final-Project
Welcome! This is the respository for the Natural Language Processing Final Project on Reddit Stock Sentiment. Below we detail the purpose of each invidiual file, all in ipynb format.

**YFinance.ipynb - **yahoo finance scraper used to output a dictionary of date-to-labels for a specified number of stocks. Data saved to yfinance.txt.<br />
**Reddit_PushShift.ipynb - **reddit pushshift scraper used to output a dictionary of date-to-posts for a specified number of stocks. Data saved to (2018 - 5thres_res_2018.txt), (2019 - 5thres_res_2019.txt), (2021 - 5thres_res_2021.txt), (2022 - 10lim_res_2022.txt).<br />
**MergeDataset.ipynb - **merges the yfinance and pushshift dataset by date to produce a text-to-label dictionary. It is saved as text_to_label.txt and both text_to_label_train.csv and text_to_label_test.csv.<br />
**Baselines.ipynb - **runs baselines of Naive Bayes, Kneighbors, SVC, and Decision Tree using the text_to_label file.<br />
**Bert.ipynb - **trains on text_to_labe_train.csv and tests on text_to_label.csv and is evaluated on how well it can predict the stock label based on the **reddit post.<br />
SentimentEvaluation.ipynb - **uses the Kaggle movie review sentiment dataset (train.tsv) to manually test accuracy of each sentiment analyzer.<br />
**SentimentAnalyzer.ipynb - **runs all four sentiment analyzers on our dataset text_to_label.txt and outputs a sentiment_array and label dictionary, with the sentiment array consisting of each of our sentiment analyzers' outputs. Data saved to sentiment_to_label.txt<br />
**SentimentMLP.ipynb - **feeds our sentiment_to_label.txt data into an MLP classifier and evaluate its performance.<br />
**All.ipynb - **runs all baselines and sentiment analyzers parallel to create a collective_array to label dictionary. This new dataset is then train and tested on MLP to evaluate the results.<br />
