# Twitter_WeRateDogs_Dataset_Analysis
With no doubt this project proved a challenge. 
The report regarding WeRateDogs Twitter account which user tweet their dogs and ratings.
The project included +2000 tweets between 2015 and 2017. 

WeRateDogs downloaded their archive of this period and sent it to Udacity so it’d be used in this project.

This project could be split into 2 major steps: 

    1. Gathering the data. 
    2. Assessing and cleaning the data.
    
## Gathering the data.
We had the data sent by WeRateDogs of the period between 2015 and 2017 ready so we simply loaded the data into the workspace (jupyter notebook).

After that comes the image_predictions provided by Udacity as this neural network was one of the projects in Udacity's Data Scientist Nanodegree, Machine Learning Engineer Nanodegree and Artificial Intelligence Nanodegree programs. 
This neural network analyzes the images in each tweet and predict the breed of the dogs and provide multiple predictions with different confidence level.

After that comes Twitter api part. I had to apply for a developer account through twitter , a process took around two days after that I managed using the code provided by the instructor to exctract the tweets’ data.
The code extract only the tweets from the dataset provided by WeRateDogs as it searched by the tweet_id of each tweet. 
After that we extract what we though a useful information from the json created which was retweet counts and favorite counts and made those along with the tweet id into a Dataframe to use later.

## Assessing and Cleaning the dataset
In this part we started assessing the three dataframes both visually and programmatically which were done to either identify quality issues and tidiness issues. 
More than eight quality issues were found and more than 2 tidiness issues.

After that the project was all about cleaning the issues found before. Several pandas method were used (i.e. info(), .drop(), .loc(), .astype(), .sample(), etc.) and many loops and functions were created to address the quality and tidiness issues. 
The final step of the cleaning process was the creation of a master data faram that contained all the cleaned data variables from the three intial dataframes. 
This dataframe was then saved in a .csv format
