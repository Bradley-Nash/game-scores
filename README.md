The Repository contains 5 files and one folder.

The "output" folder contains the csv file "MetaCritScores.csv".
The csv file is a concatenated document containing the output of the script "MetaCriticScores_Scrape_Batch_Example.ipynb"
The script was run for each page and genre in the metacritic database at the time of scraping.
The genre csv files where concatenated as detailed in "Glob_create_dataset.ipynb".

The "Best_Console.ipynb" script details lines of analysis focusing on which console was the greatest as a product of its game reviews.

The "Word_Popularity.ipynb" script details analysis focusing on what words are the most and least successful in a title based on game ratings.
-UPDATE: Contains an excecutable script to predict successful and unsuccessful future titles based on the word popularity.

The csv file contains the columns:
position = The position that the rating placed the title with its genre (1 is highest). (int)
title = The name of the game. (str)
platform = The Platform the game was released on and its rating for that platform. (str categorical)
pub_date = The date the game was released on that console. (convert to datetime)
rating = The metacritic score given to the version of the game specific to the console. (int)
genre = The genre the game is classified within (can contain duplicate entries with different genres assigned to one title version) (str categorical)
