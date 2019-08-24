# Social Media Bonanza
## YouTube vs News

ELT Project authored by: Blake Freeman, Jill Smith, Tomeka Morrison, Trong Nguyen

What is the relationship between news and social media?  In this project will we analyze news articles and YouTube posts to determine what articles earn a trending status. 

### Our data sources:
YouTube:

https://www.kaggle.com/datasnaek/youtube-new - Main Data

https://gist.github.com/dgp/1b24bf2961521bd75d6c - category ID's


News Articles:

https://www.kaggle.com/therohk/million-headlines/downloads/million-headlines.zip/8 - Main Data

### Techincal Report
Clean_News_Articles (Jupyter notebook)
* Import articles csv files using pandas and create dataframes. 
    * Files used: ArticlesJan2018, ArticlesFeb2018, ArticlesMarch2018, ArticlesApril2018
* Delete extraneous columns (refer to line 6)
* Append all four dataframes togehter to create a single dataframe
* Explore updated dataframe with function .count 
* Groupby New_Category to pull out all the category names and rename categories. (refer to lines 13 to 22)
* Saved cleaned dataframe as csv file

YouTube_Clean (Jupyter notebook)
* Import YouTube csv and Category_ID csv
* Use pandas to create dataframes from the csv files 
* Use pandas to merge the dataframes on the category_id
* Pull required columns from dataframe (refer to line 8)
* Use Datetime to update the 'trending_date' column into datetime format 
* Update the column names (refer to line 9)
* Save cleaned dataframe as csv file

Social_Media_Bonaza (Jupyter Notebook)
* Import clean YouTube_Clean and Clean_News_Artilces_v2 csv files 
* Use pandas create dataframes from csv files 
* Use pandas merged the dataframes on 'Category"
* Use JSON to convert the merged dataframe to a dictionary 
* Use pymongo added the merged dataframe to MongoDB

### Final Report 
We used MongoDB as out data was non-relational. 
Using MonoDB we explored the merged dataframe to determine 





