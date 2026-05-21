# AutoSQL
AI-powered Python application that converts natural language into executable MySQL commands using Google's Gemini API. It allows users to interact with databases conversationally, making SQL operations faster and easier without manually writing queries.

## Features
 - Natural language to SQL conversion
 - Automatic execution of generated MySQL commands
 - Interactive terminal chat interface
 - Uses Google Gemini API
 - Supports direct database interaction
 - Maintains conversational context

## Setup
 1. Clone the Repository
    ```bash
    git clone https://github.com/Ruddykraft/AutoSQL.git
    cd autosql

 2. Configure MySQL Credentials

    Open autosql.py and edit the database connection details:
    ```bash
    mydb = db.connect( host='localhost',
                       user='YOUR_USERNAME',
                       password='YOUR_PASSWORD',
                       database='YOUR_DATABASE'
                      )
 3. Add Gemini API Key
    ```bash
    gemkey.txt
    ```
    Add your Gemini API Key in this file

## Technologies Used

- mysql.connector
- google-genai

## Example Usage
```bash
Enter the SQL Command: create a table for students with id, name and marks
```
AI-generated SQL query executes automatically

## Exit
Type: 'exit' or 'quit' to close the application safely.

## Warning
This project executes AI-generated SQL commands directly on your database.
Use carefully and preferably on a testing database first.

You can also set:
```bash
mydb.autocommit = False
```
So that database doesn't auto update, you can manually ask the agent to commit changes:
```bash
Enter the SQL Command: commit the changes
```
## Future Improvements
 - GUI version
 - Better prompt engineering
 - Authentication system
