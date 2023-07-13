
07/13/2023
Elias Hagos

# NoSQL Challenge

This project focuses on analyzing the food hygiene ratings data provided by the UK Food Standards Agency. The goal is to assist the editors of a food magazine, Eat Safe, Love, in evaluating the ratings data and providing insights for their journalists and food critics.

## Part 1: Database and Jupyter Notebook Set Up

1. Start by importing the provided establishments.json file into a MongoDB database named "uk_food" and a collection named "establishments". The data import command can be found in the NoSQL_setup_starter.ipynb notebook.

2. Open the NoSQL_setup_starter.ipynb notebook in Jupyter Notebook or JupyterLab.

3. Import the necessary libraries: PyMongo and Pretty Print (pprint).

4. Create an instance of the Mongo Client to establish a connection with the MongoDB server.

5. Confirm that the "uk_food" database and "establishments" collection were created successfully. Use the appropriate MongoDB commands to list the databases and collections.

6. Retrieve and display one document from the "establishments" collection using the `find_one` method and `pprint`.

## Part 2: Update the Database

1. In the NoSQL_setup_starter.ipynb notebook, make the requested modifications to the "establishments" collection:

   - Add a new restaurant named "Penang Flavours" with the provided information.
   - Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and update the new restaurant with the BusinessTypeID.
   - Remove any establishments within the Dover Local Authority.

2. Update the data types of specific fields in the collection:

   - Use `update_many` to convert latitude and longitude to decimal numbers.
   - Use `update_many` to convert RatingValue to integer numbers.

## Part 3: Exploratory Analysis

1. Open the NoSQL_analysis_starter.ipynb notebook in Jupyter Notebook or JupyterLab.

2. Explore the database using the provided questions and queries:

   - Count the number of establishments with a hygiene score equal to 20.
   - Find establishments in London with a RatingValue greater than or equal to 4.
   - Identify the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant "Penang Flavours".
   - Determine the number of establishments in each Local Authority area with a hygiene score of 0, sorted from highest to lowest.
   - Convert the results to Pandas DataFrames and display the first 10 rows for each question.

3. Answer the questions and provide the requested information to the magazine editors.

## Files

- establishments.json: The JSON file containing the data for the establishments collection.
- NoSQL_setup_starter.ipynb: Jupyter Notebook for setting up the database and making necessary updates.
- NoSQL_analysis_starter.ipynb: Jupyter Notebook for performing exploratory analysis on the database.

## Prerequisites

- MongoDB: Ensure that you have MongoDB installed and running on your system.

##/ Setup Instructions

1. Clone the "nosql-challenge" repository to your local machine.

2. Import the establishments.json file into MongoDB using the provided data import command.

3. Open the NoSQL_setup_starter.ipynb notebook and follow the instructions to set up the database and update the collection.

4. Open the NoSQL_analysis_starter.ipynb notebook and use the provided queries to explore the database and answer the questions.

5. Provide the requested information to the magazine editors based on your analysis.
