# nosql-challenge
**Submitted by** Kaylyn Valdez-Scott **Date:** 21-NOV-2023 **Project Title:** Module 12 NoSQL Challenge

Purpose of project is to import json files to MongoDB, and use this information to manipulate and build DataFrames in Jupyter Notebook. I have been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate ratings given by the UK Food Standards Agency.

To begin, I imported the establishments.json file to MongoDB on my MAC, using the code mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json

**For Part 1 & 2** - see file labeled 'NoSQL_setup_starter-KaylynValdezScott'. 
Part 1 of the notebook aims to answer questions set out by the food magazine such as:

- List the databases you have in MongoDB. 
- Confirm that uk_food is listed.
- List the collection(s) in the database to ensure that establishments is there.
- Find and display one document in the establishments collection using find_one and display with pprint.
- Assign the establishments collection to a variable to prepare the collection for use.

Part 2 aims to answer:
An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis. 
- Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
- Update the new restaurant with the BusinessTypeID you found.
- Remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.
- Use update_many to convert latitude and longitude to decimal numbers.
- Use update_many to convert RatingValue to integer numbers.


**For Part 3** - see file labeled 'NoSQL_analysis_starter-KaylynValdezScott'.
Part 3 aims to anser more questions Eat Safe, Love has such as:

- Use count_documents to display the number of documents contained in the result.
- Display the first document in the results using pprint.
- Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.
- Which establishments have a hygiene score equal to 20?
- Which establishments in London have a RatingValue greater than or equal to 4?
- What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
- How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
