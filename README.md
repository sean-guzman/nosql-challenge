# nosql-challenge

Sean Guzman

Rutgers Data Sciences Bootcamp, Module 12 Challenge (15 May 2023)

 This module challenge utilizes MongoDB in Python and is divided into three parts:
 * Part 1: MongoDB and Jupyter Notebook Set Up
 * Part 2: Updating the Database
 * Part 3: Exploratory Analysis

**Part 1: MongoDB and Jupyter Notebook Set Up (NoSQL_setup_starter.ipynb)**
We first take a JSON file (Resources/establishments.json) containing restaurant data in the UK and import it into MongoDB using the following command in Terminal: `mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json`

Once imported, we move to our Jupyter notebook, import PyMongo and Pretty Print, and then use an instance of Mongo Client to create a connection to our new database (uk_food) and to the collection within (establishments).

**Part 2: Updating the Database (NoSQL_analysis_starter.ipynb)**
Here, we make a few requested modifications to the database:
* Add a new halal restaurant called "Penang Flavours"
* Find this new restaurant's BusinessTypeID based on its BusinessType
* Delete any listings where LocalAuthorityName contains "Dover"
* Update the type for geocode.latitude and geocode.longitude to Float for all records
* Update the type for RatingValue to Integer for all records

**Part 3: Exploratory Analysis (NoSQL_analysis_starter.ipynb)**
Lastly, we perform a few queries to answer the following questions:
* Which establishments have a hygiene score equal to 20?
* Which establishments in London have a RatingValue greater than or equal to 4?
* What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
* How many establishments in each Local Authority area have a hygiene score of 0?

