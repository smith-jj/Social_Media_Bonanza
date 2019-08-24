# Social Media Bonanza
## YouTube vs News

ELT Project authored by: Blake Freeman, Jill Smith, Tomeka Morrison, Trong Nguyen

What is the relationship between news and social media? In this project will we analyze news articles and YouTube posts to determine what articles earn a trending status. 

### Our data sources:
YouTube:

https://www.kaggle.com/datasnaek/youtube-new - Main Data
https://gist.github.com/dgp/1b24bf2961521bd75d6c - category ID's

News Articles:

https://www.kaggle.com/therohk/million-headlines/downloads/million-headlines.zip/8 - Main Data

### Techincal Report
Clean_News_Articles (Jupyter notebook)
* Import articles csv files using pandas and create dataframes. Files used: ArticlesJan2018, ArticlesFeb2018, ArticlesMarch2018, ArticlesApril2018
* Delete extraneous columns: 'articleID', 'articleWordCount', 'byline', 'documentType', 'headline','keywords', 'multimedia', 'newDesk', 'printPage', 'pubDate','sectionName', 'snippet', 'source', 'typeOfMaterial', 'webURL'
* Append the dataframes togehter to create a single dataframe
* Explore updated dataframe with function .count 
* Groupby New_Category to pull out all the category names and rename categories. (refer to lines 13 to 22)
* Saved updated clean dataframe as csv 

YouTube_Clean (Jupyter notebook)
* Import YouTube csv and Category_ID csv
* Use pandas to create dataframes from the csv files 
* Use pandas to merge the dataframes on the category_id
* Use Datetime to update the 'Date' column into datetime format 
* Update the column names 
* Saved as csv file

Social_Media_Bonaza (Jupyter Notebook)
* Import clean YouTube and Clean_News_Artilces_v2 csv files and create dataframes from files 
* Use pandas merged the dataframes on 'Category"
* Using pymongo added the merged dataframe to MongoDB






