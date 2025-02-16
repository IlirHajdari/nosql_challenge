# UK Food Hygiene Ratings Analysis

## NOTE ##
The starter code for this assignment was provided by the course/class, which is why I did not rename the folders and continued on from where the course left off.

## Description
This project analyzes **UK Food Hygiene Ratings** using **MongoDB** and **PyMongo**. The goal is to extract, clean, and explore food hygiene data to help journalists and food critics identify key trends for their articles.

## Summary

### Part 1: Database and Jupyter Notebook Setup
The first part of this project involves setting up a **MongoDB NoSQL database**, importing data, and verifying that the database is correctly structured.

#### Key Deliverables:
- Import the **establishments.json** dataset into a MongoDB database named `uk_food`.
- Verify that the `establishments` collection is properly loaded.
- Use **PyMongo** to connect to the database.
- Perform initial data checks, including:
  - Listing all databases and collections.
  - Retrieving a sample document from the dataset.

### Part 2: Database Updates
Before performing any analysis, modifications were made to the database based on the editors' requests.

#### Key Deliverables:
- **Insert a new restaurant** (`Penang Flavours`) into the database.
- **Retrieve and update** the `BusinessTypeID` for `"Restaurant/Cafe/Canteen"`.
- **Remove all establishments** from the database that fall under the **Dover Local Authority**.
- **Convert data types**:
  - Change `latitude` and `longitude` from **strings** to **decimal numbers**.
  - Convert `RatingValue` to an **integer** while setting non-numeric values to `null`.

### Part 3: Exploratory Analysis
Once the database was properly structured, various queries and aggregations were performed to extract meaningful insights.

#### Key Deliverables:
- Identify **all establishments** with a hygiene score of **20**.
- Find **all establishments in London** with a `RatingValue ≥ 4`.
- Retrieve the **top 5 establishments** closest to `"Penang Flavours"` with a `RatingValue = 5`, sorted by **lowest hygiene score**.
- **Group establishments** by Local Authority and count how many have a hygiene score of **0**.
- **Sort Local Authorities** by the number of establishments with a hygiene score of **0** in descending order.

## Requirements

### Tools and Libraries

**Database:**
- MongoDB
- PyMongo

**Python Libraries:**
- Pandas
- Pretty Print (`pprint`)

## Contact Information

For questions or additional information, reach out to me at:
- **Email:** ilir.hajdari111@gmail.com