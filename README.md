# TechCare Solutions Riwi - Database Project

## Project Description
This project takes a messy Excel sheet with repeated data and turns it into a clean, organized MySQL database. This prevents errors like repeated clients or duplicate service orders.

## Technologies Used
*   **Database Engine**: MySQL
*   **Tool**: MySQL Workbench
*   **Language**: SQL

## Database Engine
The project runs entirely on **MySQL** inside MySQL Workbench.

## Explanation of the Normalization Process
To fix the data and organize it, we followed three simple steps:
1.  **First Step (1FN)**: Separated everything into rows and columns with unique IDs.
2.  **Second Step (2FN)**: Created specific tables for each topic (`CITY`, `BRANCH`, `CLIENT`, `TECHNICIAN`, `CATEGORY`, `EQUIPMENT`, `SERVICETYPE`).
3.  **Third Step (3FN)**: Connected the tables using Foreign Keys so everything links together without errors.

## Database Structure
The database has 8 simple tables:
*   `CITY`: The cities where we operate.
*   `BRANCH`: The offices or offices in each city.
*   `CLIENT`: The clients assigned to a branch.
*   `TECHNICIAN`: The technicians doing the work.
*   `CATEGORY`: Types of equipment (Laptop, Desktop, etc.).
*   `EQUIPMENT`: The specific devices being fixed.
*   `SERVICETYPE`: Types of service (Preventive, Corrective).
*   `ORDERWORKING`: The main table that records every maintenance job done.

## Entity Relationship Diagram
*   Cities have Branches.
*   Branches have Clients.
*   Categories have Equipment.
*   Clients, Technicians, and Equipment all connect inside `ORDERWORKING`.

## Database Creation Instructions
1. Open MySQL Workbench.
2. Run the table creation code (DDL).
3. Check the left panel to see the tables created under your database.

## Data Loading Instructions
To insert data without errors, you must paste the code in this exact order:
1. Insert Cities and Service Types.
2. Insert Branches.
3. Insert Clients.
4. Insert Categories and Equipment.
5. Insert Technicians.
6. Insert the Work Orders (`ORDERWORKING`) at the very end.

## Explanation of each SQL Query
The queries help the company make better decisions:
*   **Query 1**: Shows how many orders each technician handled.
*   **Query 2**: Shows which cities requested the most services.
*   **Query 3**: Shows which type of service is the most popular.
*   **Query 4**: Shows which devices break down the most.
*   **Query 5**: Shows our top clients with the most orders.
*   **Query 6**: Shows the workload of each branch office.

## Developer Information
*   **Full Name**: Cristian David Silva Quintero
*   **Clan**: Cumbia
