# no-sql Challenge
## Background
The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

## Part 1: Database and Jupyter Notebook Set Up
The code for this section can be found in the NoSQL_setup_starter.ipynb file.
First I imported the data provided in the establishments.json file from my Terminal and named the database uk_food and the collection establishments.
Then Within my notebook, I imported the libraries I needed: PyMongo and Pretty Print (pprint).
Next I created an instance of the Mongo Client.
Then I confirmed the creation of the database and loaded the data properly, using the following steps:
* Listed the databases I have in MongoDB to confirm that uk_food is listed.
* Listed the collection(s) in the database to ensure that establishments is there.
* Found and displayed one document in the establishments collection using find_one and displayed it with pprint.
* Assigned the establishments collection to a variable to prepare the collection for use.

<img width="1295" alt="Screenshot 2024-04-01 at 12 31 25 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/0429bf6c-1a4a-4570-b99c-a2a13d237443">
<img width="1295" alt="Screenshot 2024-04-01 at 12 31 38 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/8256841f-e77a-4c0c-a61d-8f33239c6e8c">
<img width="1295" alt="Screenshot 2024-04-01 at 12 31 55 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/98231fe4-901a-4432-b6b0-5a0ce1924dc2">
<img width="1295" alt="Screenshot 2024-04-01 at 12 32 14 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/f234e3f7-73b1-4075-b3e4-6536718b27bd">


## Part 2: Update the Database
The code for this section can be found in the NoSQL_setup_starter.ipynb file. 
### Instructions
The magazine editors have some requested modifications for the database before you can perform any queries or analysis for them. Make the following changes to the establishments collection:
* An exciting new halal restaurant just opened in Greenwich, but hasn't been rated yet. The magazine has asked you to include it in your analysis.

<img width="1295" alt="Screenshot 2024-04-01 at 12 35 54 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/5f53a966-9d94-495c-9e0a-38f2c1174a5f">
<img width="1273" alt="Screenshot 2024-04-01 at 12 36 11 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/88cece36-2b06-47bc-8293-d637e69988dd">


* Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.

<img width="1273" alt="Screenshot 2024-04-01 at 12 37 51 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/394fca90-a370-4ddc-aed8-cc4d7fb7488e">

* Update the new restaurant with the BusinessTypeID you found.

<img width="1269" alt="Screenshot 2024-04-01 at 12 38 36 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/20306795-22d0-40d4-8f62-ce051297d8a6">

* The magazine is not interested in any establishments in Dover, so check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database, and check the number of documents to ensure they were deleted.

<img width="1269" alt="Screenshot 2024-04-01 at 12 39 29 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/2b440a65-6cb7-46a7-add3-0dbcb465c018">
<img width="1269" alt="Screenshot 2024-04-01 at 12 39 44 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/f8e3e155-7aa2-4953-8cee-4c5b7db013e2">


* Some of the number values are stored as strings, when they should be stored as numbers, change them.

<img width="1275" alt="Screenshot 2024-04-01 at 12 40 35 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/034434ff-05ff-4246-9f9f-a8844249958b">
<img width="1275" alt="Screenshot 2024-04-01 at 12 40 44 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/16d46630-25d3-4eaf-8419-1cc72e228b9c">

## Part 3: Exploratory Analysis
The code for this section can be found in the NoSQL_analysis_starter.ipynb file.
### Background
Eat Safe, Love has specific questions they want you to answer, which will help them find the locations they wish to visit and avoid.
### Instructions
Answer the following questions:
* Which establishments have a hygiene score equal to 20?

<img width="1275" alt="Screenshot 2024-04-01 at 12 48 24 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/a729fb1b-298a-4092-892b-33c0482f02e9">
<img width="1275" alt="Screenshot 2024-04-01 at 12 48 39 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/8baea478-583f-4d1c-aa4b-e60d18bd416b">
<img width="1384" alt="Screenshot 2024-04-01 at 12 48 57 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/e0edfd38-a861-48fa-8f3c-95022137123c">


* Which establishments in London have a RatingValue greater than or equal to 4?


<img width="1390" alt="Screenshot 2024-04-01 at 12 49 43 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/897ccf08-f8df-4890-b192-69f41876cc73">
<img width="1390" alt="Screenshot 2024-04-01 at 12 50 01 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/bd4642f9-38b5-4cc8-ae64-b36e5bf4971f">
<img width="1390" alt="Screenshot 2024-04-01 at 12 50 19 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/825b8fd2-b56b-4b56-8761-15e287ff6bd1">
<img width="1390" alt="Screenshot 2024-04-01 at 12 50 34 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/cf080249-71df-4966-927d-aa7120712a3f">

* What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

<img width="1396" alt="Screenshot 2024-04-01 at 12 51 15 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/de6b8f68-0089-4f64-bd47-de7a13409733">
<img width="1396" alt="Screenshot 2024-04-01 at 12 51 29 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/88b7ca52-8974-47c4-8f24-b549f8f30d47">
<img width="1396" alt="Screenshot 2024-04-01 at 12 51 40 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/0c47a3ff-d1ef-41fb-89e1-de5a2b10e20c">
<img width="1396" alt="Screenshot 2024-04-01 at 12 51 53 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/fb07ec86-6760-4c62-9308-86ecca6d8a38">

* How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

<img width="1396" alt="Screenshot 2024-04-01 at 12 52 33 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/92e0f392-52c4-419d-89a4-df6093c58a04">
<img width="1396" alt="Screenshot 2024-04-01 at 12 52 47 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/55079101-e32d-40eb-b717-93ee44d308ca">
<img width="1396" alt="Screenshot 2024-04-01 at 12 52 56 PM" src="https://github.com/mattflanagan2/nosql-challenge/assets/146908072/b52a519c-d528-431a-8e1f-e5220cb746c2">

