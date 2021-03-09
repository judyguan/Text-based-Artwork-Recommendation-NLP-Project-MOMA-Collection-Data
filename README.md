# Text-based-Artwork-Recommendation-NLP-Project-MOMA-Collection-Data
## Part1: Business Context

Targeted Industry/Company: Art Auction House(Sotheby's)

Background: 
• 24% Growth of Sotheby’s online market in 2018 and $220 billion revenue it brought (Sotheby’s 2018 Anuual Report)
• Growth in middle market and young collectors who have interests yet not too much profound knowledge of art 
• Traditional Approach of suggesting artworks: Specialists contacting potential buyers based on their relationship for specific upcoming lots 

Goal:
To help collectors discover art more easily through the platform by suggesting RELEVANT pieces of art based on word descriptions (similar theme/topic) on artists or artworks that you have searched for or bought. 

## Part2: NLP Techniques and Methods
• Generated an NER analysis for each artwork description using IBM Natural Language Understanding API in Python
• Conducted feature extraction based on semantic sentiment analysis
• Applied topic modeling to cluster artwork titles into topics
• Constructed Word2Vec model to calculate similarity scores based on artworks’ titles and descriptions to generate top 15 similar
artworks for a given artwork from database
