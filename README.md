# Instagram-bot-classifier-DIIGData_WIRLF23
Python based neural network classifying instagram user profiles as real IDs or spam/bot IDs.


Machine learning model classifying instagram profiles as real or spam. Neural network implemented with input layer, 4 Dense layers, 3 dropout layers and a softmax-activated output layer. Trained on training dataset of ~600 Instagram IDs. Data used in training the model includes columns: profile_pic (boolean),nums/length username,fullname words,nums/length fullname,name==username (boolean),description length,external URL,private (boolean),#posts,#followers,#follows,fake(boolean). Referenced from Ryan Ahmed, Ph.D. through Coursera. Tested using custom dataset acquired through kaggle of 120 Instagram IDs with an accuracy of 88%. 

Complete Python script providing code for EDA, visualizations, creating the model, training the model, assessing performance etc.

Implemented in the context of analyzing Wellness in Real Life (WIRL)'s instagram account and following, as part of Duke Impact Investing Group's Data Division of Fall 2023. For more context: https://docs.google.com/presentation/d/10c87pC0KekE63q9Y9dqYh9CfxP3eSOglRL7HZfnHvDc/edit?usp=sharing 

Used PhantomBuster (publicly available chrome extension) to scrape information about WIRL's 7748 followers on instagram. Obtained comprehensive dataset on follower information with 29 features and 225,000 data points. Wrangled scraped dataset to fit the data format the neural network was trained on. 

Some of these transformations included:

Binary indicators to check:
If the full name and username are identical.
If the account mentions a website.
If the account is private.

Calculating statistics such as:
The ratio between the number of numerical characters to the length of username.
The ratio between the number of numerical characters to the full name.
Number of words in the Full Name and Description Length 

This repo contains the python code to train and assess the model, the training dataset used, the testing dataset used, scraped data on WIRL and predictions based on applications of results. 




