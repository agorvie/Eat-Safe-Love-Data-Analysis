# Eat Safe, Love Data Analysis
## Project Description
The UK Food Standards Agency evaluates various establishments across the United Kingdom, providing them with food hygiene ratings. In this project, I will analyze and manipulate this rating data to assist the editors of the food magazine "Eat Safe, Love" in deciding where to focus future articles. The analysis will be perform in three parts:

### Part 1: Database and Jupyter Notebook Setup
In this section, I will set up the database and Jupyter Notebook environment. I will import the provided data, confirm its proper import, and prepare the data for analysis.

    1. Import the data from the "establishments.json" file into a MongoDB database named "uk_food" and a collection named "establishments".
    2. Import the necessary Python libraries, including PyMongo and Pretty Print (pprint).
    3. Create an instance of the MongoDB client.
    4. Confirm the database and collection creation.
    5. Find and display one document from the "establishments" collection.
    6. Assign the "establishments" collection to a variable for further use.

### Part 2: Update the Database
In this section, I will make specific modifications to the database as requested by the magazine editors.

    1. Add information about a new halal restaurant, "Penang Flavours," which has not been rated yet, to the database.
    2. Find the "BusinessTypeID" for "Restaurant/Cafe/Canteen" and update the new restaurant with this information.
    3. Check how many establishments are in the "Dover" Local Authority, remove them from the database, and confirm their deletion.
    4. Convert certain number values from strings to numbers using update_many.

### Part 3: Exploratory Analysis
In this section, I will answer specific questions provided by "Eat Safe, Love" through data exploration.

    1. Identify establishments with a hygiene score equal to 20.
    2. Find establishments in London with a "RatingValue" greater than or equal to 4.
    3. Determine the top 5 establishments with a "RatingValue" of 5, sorted by the lowest hygiene score, nearest to the new restaurant "Penang Flavours."
    4. Calculate the number of establishments in each Local Authority area with a hygiene score of 0, sort the results from highest to lowest, and display the top ten local authority areas.

## Project Structure
The project will be organized into three main parts, each corresponding to the sections outlined above:

    * Part1_NoSQL_setup.ipynb: Jupyter Notebook for Database and Jupyter Notebook Setup.
    * Part2_NoSQL_modifications.ipynb: Jupyter Notebook for Updating the Database.
    * Part3_NoSQL_analysis.ipynb: Jupyter Notebook for Exploratory Data Analysis.
    
## Data Sources
The primary data source for this project is the "establishments.json" file, containing information about food establishments and their ratings.
#### References
UK Food Standards Agency (2022). UK food hygiene rating data API. https://ratings.food.gov.uk/open-data/en-GBLinks to an external site.. Contains public sector information licensed under the Open Government Licence v3.0Links to an external site.
Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).

## Technologies Used
- MongoDB for database storage.
- Python with PyMongo for data manipulation.
- Jupyter Notebook for code execution and documentation.
- Pandas for data analysis and visualization.
  
How to Run the Project
Follow the instructions in each Jupyter Notebook (Part1, Part2, Part3) to execute the code and perform the specified tasks. Ensure that MongoDB is properly installed and running on your system for database operations.
