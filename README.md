# Sakila DVD Rental database Analysis


## Introduction

In this project, we have queried the Sakila DVD Rental database. The Sakila Database holds information about a company that rents movie DVDs. For this project, we have queried the database to gain an understanding of the customer base, such as what the patterns in movie watching are across different customer groups, how they compare on payment earnings, and how the stores compare in their performance. For assistance in the queries, the schema for the DVD Rental database was used as given in the `dvd-rental-erd-2.pdf`.


## Local Environment Setup

Follow the steps provided below to setup the local environment with **PostgreSQL** and database

**Step 1. Downloading PostgreSQL**

First, we will need to install PostgreSQL on your local machine. The instructions below provide detailed description of the steps we need to take.

**Installing PostgreSQL for Windows:**

http://www.postgresqltutorial.com/install-postgresql/

**Installing PostgreSQL for Mac OS:**

https://www.postgresql.org/download/macosx/

**Note:** We need to write down the database superuser (postgres) password as we will need it to create the Sakila database once we have installed the PostgreSQL server.

**Step 2. Downloading Sakila database**

Once PostgreSQL server is installed, we will need to download the Movie database from this page: [PostgreSQL Sample Database](http://www.postgresqltutorial.com/postgresql-sample-database/)

Scroll down and click on the orange "Download DVD Rental Sample Database" button.

This will download a zipped file, and you will need to extract the `dvdrental.tar file`.

**Step 3. Loading database**

The next step is to load the DVD Rental database into our PostgreSQL server on our machine. We recommend using the **PgAdmin tool**. We can find the instructions to do so on the following link: [Load PostgreSQL Sample Database](http://www.postgresqltutorial.com/load-postgresql-sample-database/).

The instructions are down ⅓ on this page under the header **“Load the DVD Rental database using pgAdmin tool”** .

Now, we need to follow the instructions all the way through the header titled **"Verify the loaded sample database."**

Once we have followed the instructions through the end of **"Verify the loaded sample database."**, we have now loaded the `dvdrental` sample database into our local PostgreSQL database server.

**Step 4. Connecting back to the PostgreSQL server:**

Now, we will relaunch PgAdmin III and click on the PostgreSQL server within the Object browser and enter our superuser (postgres) password.

**Step 5. Connecting to the DVD rental database:**

Next, we will click on the plus sign next to Databases to access the DVD rental database.

**Step 6. Choose the DVD Rental database**

Choose the `dvdrental` database under Databases.

We are now linked to the DVD rental database.

**Step 7. Running Queries on your dvdrental database**

Now, we are ready to run some queries. For that, we need to click on the SQL icon with a magnifying glass

## Questions to work upon for analysis

**Question 1**

We want to understand more about the movies that families are watching. The following categories are considered family movies: Animation, Children, Classics, Comedy, Family and Music.

**Create a query that lists each movie, the film category it is classified in, and the number of times it has been rented out.**

**Question 2**

Now we need to know how the length of rental duration of these family-friendly movies compares to the duration that all movies are rented for. **Can you provide a table with the movie titles and divide them into 4 levels (first_quarter, second_quarter, third_quarter, and final_quarter) based on the quartiles (25%, 50%, 75%) of the rental duration for movies across all categories?** Make sure to also indicate the category that these family-friendly movies fall into.

**Question 3**

Finally, provide a table with the family-friendly film category, each of the quartiles, and the corresponding count of movies within each combination of film category for each corresponding rental duration category. The resulting table should have three columns:

- Category
- Rental length category
- Count

**Question 4**

We would like to know who were our top 10 paying customers, how many payments they made on a monthly basis during 2007, and what was the amount of the monthly payments. **Can you write a query to capture the customer name, month and year of payment, and total payment amount for each month by these top 10 paying customers?**





