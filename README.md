# nosql-challenge
------------------------------

OBJECTIVE:
    Evaluate some of the ratings data from a food magazine in order to help their journalists and food critics decide where to focus future articles.

----------------------------------------------------------------------------------
*THIS CODE CAN BE FOUND WITHIN THE FOLLOWING FILE: "RL_NoSQL_setup.ipynb"*
# PART ONE: Database and Jupyter Notebook Set-up

-Imported data provided in establishments.json file from Terminal, named the database 'uk_food' and the collection 'establishments.' 
(Copied the text used to import your data from Terminal to a markdown cell in notebook)

-Within Jupyter notebook, named imported data as variable 'food_db,' and named establishments as 'collection.'


----------------------------------------------------------------------------------

# PART TWO: Updating the Database

-Added and updated entry for new restaurant 'Penang Flavours.'
-Deleted all documents where LocalAuthorityName was 'Dover.'
-Converted latitude and longitude to decimal numbers.


----------------------------------------------------------------------------------
*THIS STARTS A NEW FILE WITHIN THE REPOSITORY, TITLED "RL_NoSQL_analysis.ipynb"*
# PART THREE: Exploratory Analysis

Notes:
RatingValue refers to the overall rating decided by the Food Authority and ranges from 1-5. The higher the value, the better the rating. Note: This field also includes non-numeric values such as 'Pass', where 'Pass' means that the establishment passed their inspection but isn't given a number rating.

The scores for Hygiene, Structural, and ConfidenceInManagement work in reverse. This means, the higher the value, the worse the establishment is in these areas.

-Generated queries and aggregation pipelines to address the following questions:

Which establishments have a hygiene score equal to 20?

Which establishments in London have a RatingValue greater than or equal to 4?

What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.