Database Layer Overview: 

Schema -> Defines structure of database
    -Defines what data exists
    -Defines how data is organized
    -(doesn't contain the data itself)

Migrations -> Version control for changes to database
    -Create a migrations file for each function in data access layer that modifies the database

Seed -> Insersts initial data into database (random sample data for example)

Keep database seperate on server, database layer only contains instructions for the database