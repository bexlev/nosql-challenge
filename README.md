# nosql-challenge
------------------------------

OBJECTIVE:
    Evaluate some of the ratings data from a food magazine in order to help their journalists and food critics decide where to focus future articles.

----------------------------------------------------------------------------------

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

# PART THREE: Exploratory Analysis

Notes:
RatingValue refers to the overall rating decided by the Food Authority and ranges from 1-5. The higher the value, the better the rating. Note: This field also includes non-numeric values such as 'Pass', where 'Pass' means that the establishment passed their inspection but isn't given a number rating.

The scores for Hygiene, Structural, and ConfidenceInManagement work in reverse. This means, the higher the value, the worse the establishment is in these areas.

-Converted the result to a Pandas DataFrame