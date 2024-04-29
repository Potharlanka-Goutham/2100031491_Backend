# 2100031491_Backend

IN TASK 1:

Insert location data (street address, city, state/province, country code) into the locations table.
Insert country data (country ID, country name, region ID) into the countries table.
Find address details (location ID, street address, city, state/province) based on a specified country name.

How to Run
Ensure you have Python installed on your system.
Install the mysql-connector-python package using pip: pip install mysql-connector-python
Update the MySQL connection details (host, user, password, database) in the script to match your MySQL setup.
Run the script using Python: python Task1.py

Follow the prompts to interact with the menu options:
Enter option 1 to insert location data.
Enter option 2 to insert country data.
Enter option 3 to find address details for a specific country.
Enter option 4 to exit the program.

Overview of Sections
Database Connection: Establishes a connection to the MySQL database.
Table Creation: Creates the locations and countries tables if they don't already exist.

Data Insertion Functions:
insert_location_data: Prompts the user to input location data and inserts it into the locations table.
insert_country_data: Prompts the user to input country data and inserts it into the countries table.

Address Retrieval Function:
find_address: Prompts the user to enter a country name and retrieves address details for that country using a join between the locations and countries tables.

Main Menu Loop: Presents a menu to the user with options to interact with the database.
Menu Action Mapping: Maps menu options to corresponding functions using a dictionary.
Error Handling: Catches and displays errors occurring during database operations.
Closing Connections: Ensures proper closure of database connections and cursors

IN TASK 2:

Prompt the user to input a country name.
Query the database to find the corresponding country ID based on the provided country name.
Retrieve address details (location ID, street address, city, state/province) for the specified country.
Display the retrieved address details in the console.

How to Use
Ensure you have Python installed on your system.
Install the mysql-connector-python package using pip: pip install mysql-connector-python
Update the MySQL connection details (host, user, password, database) in the script to match your MySQL setup.
Run the script using Python: python Task2.py
Follow the prompts to input a country name and retrieve the address details.

Overview of Script
Database Connection: Connects to a MySQL database using the provided connection details (host, user, password, database).
User Input: Prompts the user to input a country name.
Country ID Retrieval: Queries the countries table to find the corresponding country_id based on the provided country name.
Country ID Validation: Checks if a matching country_id is found. If not, prints a message indicating that the country is not found.
Address Retrieval: If a matching country_id is found, queries the locations table to retrieve the address details (location ID, street address, city, state/province) for the specified country.
Output: Displays the retrieved address details in the console, including the country name, location ID, street address, city, and state/province.
Error Handling: Catches and prints any MySQL errors that occur during database operations.
Closing Connections: Ensures proper closure of the database cursor and connection.
