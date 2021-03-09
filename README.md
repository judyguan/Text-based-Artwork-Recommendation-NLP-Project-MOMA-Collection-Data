# Text-based-Artwork-Recommendation-NLP-Project-MOMA-Collection-Data
## Part1: Business Context

Targeted Industry/Company: Art Auction House(Sotheby's)
Sotheby’s is one of the world’s largest auction houses and brokers of fine art, jewelry, wine, automobiles, and real estates. It manages private sales, art auctions as well as art financing. Beginning in 2000, Sotheby’s became the first international auction house to hold online auctions.(Sothebys.com)

Background: 
• 24% Growth of Sotheby’s online market in 2018 and $220 billion revenue it brought (Sotheby’s 2018 Anuual Report)
• Growth in middle market and young collectors who have interests yet not too much profound knowledge of art 
• Traditional Approach of suggesting artworks: Specialists contacting potential buyers based on their relationship for specific upcoming lots 

Goal:
To help collectors discover art more easily through the platform by suggesting RELEVANT pieces of art based on word descriptions (similar theme/topic) on artists or artworks that you have searched for or bought. 

Note: Since the internal dataset is not available to the public, we will use a similar dataset of MOMA’s collection catalogue to run and test our proposed artwork recommendation system.

## Part2: Data Source
Data source: Collection - dataset by moma (https://data.world/moma/collection)
It represents all of the works that have been acquired into MoMA’s collection and includes metadata for each work with 29 columns

Collection specific columns: 'Title', ‘Medium’, 'Dimensions','Classification', 'Department',  'DateAcquired', 'Cataloged', 'URL', 'ThumbnailURL',  'Circumference (cm)', 'Depth (cm)', 'Diameter (cm)', 'Height (cm)',  'Length (cm)', 'Weight (kg)', 'Width (cm)', 'Seat Height (cm)','Duration (sec.)'.

Artist specific columns: 'Artist', 'ArtistBio', 'Nationality',  'BeginDate', 'EndDate', 'Gender'.

“Text/Description” will be added to the dataset by reading the article body for each URL.


## Part3: NLP Techniques and Methods
• Generated an NER analysis for each artwork description using IBM Natural Language Understanding API in Python
• Conducted feature extraction based on semantic sentiment analysis
• Applied topic modeling to cluster artwork titles into topics
• Constructed Word2Vec model to calculate similarity scores based on artworks’ titles and descriptions to generate top 15 similar
artworks for a given artwork from database

## Part4: Evaluation Criteria
Model Evaluation:
For intra-model tuning and evaluation, metrics such as Log-loss,Perplexity,and cosine distances will be used.
For overall platform performance evaluation, percentage of relevant recommendations amongst the top-15 results will be used as the metric.

Business Impact Evaluation: 
In order to measure success and utility of the platform once launched, we will use the following measure(s): click through rate on recommendation results and sell rate on recommendation results.


