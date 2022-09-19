PREREQUISITES - 
1) Jupyter NoteBook installed.
2) Postgresql installed and configured - https://www.postgresql.org/download/ 
3) Remember the user login credentials. The same credentials will be used to connect to the server
4) The user does not have to create a database or table. These operations will be performed progamatically 
in the Jupyter Notebook

IMPLEMENTATION - 

1) The original data contains restaurant details (restaurant name, opening and closing times and days). The data is in the following format - 

![image](https://user-images.githubusercontent.com/77750662/190984957-9fec7a04-e60d-45fe-b5d9-f445d2993d87.png)

2) This data is then cleaned using pandas profiling as shown below - 

![image](https://user-images.githubusercontent.com/77750662/190985649-83236265-a27f-4b3b-939c-45828e194cc6.png)

3) A connection to a PostgreSQL database server is established via a python function. The cleaned data is then pushed to the database. 

4) Finally a python function is created that contains the PostgreSQL query to retrieve the names of restaurants open at a date specified by the user (local time of the user).
