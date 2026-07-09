# User Management Web Application</h1>

## Project Overview
This is a full stack web application built to manage user details through a simple web interface. It allows users to add new records such as name and email 
via a form and view all stored users and details in a table.

##Technologies Used
- **Frontend:** HTML, CSS
- **Backend:** Python (Flask)
- **Database:** SQLite
- **Tools:** VS Code, Browser

## Project Flow
1. The user opens the home page (index.html), which displays a form to enter Name and Email.
2. On submitting the form, the data is sent via a POST request to the Flask backend.
3. Flask receives the form data and inserts it into the SQLite database (database.db) using an INSERT SQL query.
4. After inserting, the page redirects back to the home route.
5. On every page load , Flask fetches all existing users from the database using a SELECT query.
6. The fetched data is passed to the HTML template using Jinja2 templating and displayed in a table.
7. Basic CSS (style.css) is used to style the form, table, and headings for a display.
