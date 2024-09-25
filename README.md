# 4.1_Artist-Band_p2
In this individual assignment, you will demonstrate how to use a SQL script to write more advanced SQL SELECT queries to retrieve information from the band database similar to the one you created in team assignment 3.2.

Your task is to create a single .sql script that contains the SQL queries that produce the output for the following 5 questions.

Download this script: assignment41.sql.Download assignment41.sql.

IMPORTANT NOTE: This script will create a new set of tables and a new dataset compared to your submission for the previous assignment. Don't worry: we will still be able to grade Assignment 3.2 by running the script that you turned in. However, if for any reason you have not submitted assignment 3.2, consult with your instructor.
After reading the queries that you need to write, you may need to edit the INSERT statements in the script as necessary to ensure you have adequate data.
Add the SELECT queries for this assignment to the end of the script.
Run your copy of the script in your individual MySQL database.
Do not hard code! In other words, do not use specific IDs in your WHERE instead of writing a query that works for any data added that might be added to the tables. Don't just look at the data, figure out the answer and then print that specific name or ID

Whenever you're asked for an artist's full name, combine the parts of their name into one value  - i.e. if fname = "Jane" and lname = "Doe", return "Jane Doe".

# Question 1
For each artist who is currently in a band and is under 30 years old: *

Return the artist’s full name, gender, date of birth (formatted like  "06/12/2019"), and the name of the band they are in with date joined formatted like "July 18, 2022".

Order the results by artist name

* You will not get full points if you just say something like DOB > '1992-03-23' (hard coded thirty years ago today). The query would not age well!

# Question 2
For all artists who are currently in a band:

Return the artist’s full name (as a single value), the band name, and how long in years the artist has been in the band. The artist should only be shown once for each band.

(Hint: Remember that the data might include an artist who left a band and then rejoined. That is the challenge here!)

# Question 3
For each band that currently has a female member:

Return the name of the band and each artist's full name (as a single value).

Order by band name and artist name.

Comment: It is fairly easy to write a query that returns just the female members who are currently in bands (12 rows); doing this correctly will earn you the 7 points for this question. However, the question is really asking for all current members of bands that currently have a female member (20 rows); I don't believe that can be done without a subquery, so if you do some research and figure out how to do the subquery, you can earn 2 bonus points.

# Question 4
Find the album title, band name, format, and total length of all albums released since January 1, 2000.

Order from longest to shortest.

Try to return the format as the word "single" or "double" rather than just the stored value "s" or "d". (Google 'mySQL IF() function'.)

Try to get the total length to look like a reasonable time value rather than just a big number. This is hard! Google "summing time values in MySQL".

# Question 5
For all bands:

Return how many artists are currently in the band, how many artists have ever been in the band (be careful not to count the same artists multiple times if they've left and rejoined) and the number of albums the band has made. This is tricky! There are a number of ways you can approach this.

Order by band from A-Z.
