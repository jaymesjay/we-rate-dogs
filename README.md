# We-rate-dogs Data Analysis
## by James Okoro

## Dataset
In this project, the dataset to be wrangled, analyzed and visualized is the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. Three different methods would be used to gather them since they are of different file formats and sources:
- Directly download the WeRateDogs Twitter archive data (twitter_archive_enhanced.csv)
- Use the Requests library to download the tweet image prediction (image_predictions.tsv)
- Use the Tweepy library to query additional data via the Twitter API (tweet_json.txt)

## Data Cleaning
In this section, using both visual and programmatic assessment, we would detect the quality and tidiness issues associated with this data.

### Quality issues
These are issues that are imbedded in the content of the data. A high quality data should be complete, accurate, valid and consistent. From the assessment above, we observed the quality issues below:
- Irrelevant data related to retweets and status replies in df_archive
- Erroneous datatypes in the dataframes
- Invalid dog names
- Inaccurate dog ratings
- Hyperlink not extracted from source
- Irrelevant url at the end of the text in df_archive
- Inconsistency in letter case of dog breed in df_image
- Irrelevant columns
- Non dog image predictions

### Tidiness issues
Untidy data commonly referred to as messy data have structural issues. The following tidiness issues were observed during the assessment:
- Numerator and denominator for ratings should be in one column
- Dog stage should be in one column
- Merge tables with tweet_id as primary key
After cleaning, the master dataframe (df_master) has 1,666 entries and 19 variables and it would be further analyzed in this section.

## Key Insights
WeRateDogs tweet archive was wrangled and analyzed and below are some of the conclusions:
- The major source of tweets is Twitter for iPhone.
- Noticable top breeds being tweeted are, Golden retriver and Labrador Retriever.
- Most common stage of dog is pupper
- Most dogs were rated 10, 11 and 12
- Retweets and Favorites are highly correlated
