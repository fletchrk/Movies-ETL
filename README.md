# Movies-ETL
Mod 8 Repository

## Project Overview
Amazing Prime asked to have an analyst create an automated pipeline that takes in data from Wikipedia, MovieLens and Kaggle then apply appropriate transformations and load data into existing tables. 

## Summary
The analyst consisted of performing four technical deliverables which included:
1.	Develop an ETL function to read three data files in Python
2.	Extract and Transform the Wikipedia data in Python
3.	Extract and Transform the Kaggle data in Python
4.	Create a movie database in SQL

### Deliverable 1
Deliverable 1 created an ETL function was developed to read data files and convert files to DataFrame. The function converted the Wikipedia JSON file to a Pandas DataFrame, convert the Kaggle metadata file to a Pandas DataFrame and the last convert was with the MovieLens ratings data to a Pandas DataFrame. 

### Deliverable 2
Deliverable 2 was set up to filter out the wiki_movies_df DataFrame, to catch errors while extracting IMDb IDs with a regular expression and dropping duplicate IDs. The box office column, budget column, release data column, and the running time column in the wiki_movies_df were cleaned up and a new Pandas DataFrame was displayed.

### Deliverable 3
Deliverable 3 helped extract and transform the Kaggle metadata. The metadata was cleaned and merged with the Wikipedia DataFrame. The following tasks were performed after the Wikipedia and Kaggle DataFrames to create a new DataFrame titled movies_df:
•	All the columns that were not necessary were dropped
•	A function was used to fill in the missing Kaggle data
•	The movies_df DataFrame was filtered to keep specific columns
•	Columns in the movies_df DataFrame were renamed.
Deliverable 3 also extracted and transformed the MovieLens ratings data by using the following ETL function:
•	The ratings counts were cleaned up
•	The movies_df DataFrame was merged with the cleaned ratings DataFrame creating a new DataFrame titled movies_with_ratings_df.
•	The empty values in the movies_with_ratings_df DataFrame were filled with zeros.

### Deliverable 4
Deliverable 4 requirements were to replace a pre-existing movies table in SQL with the new movies_df DataFrame data. Another requirement for deliverable 4 was to add the ratings table to SQL database. The final requirement for deliverable 4 was to add code to determine the elapsed time that it took to download the ratings data into SQL>
