Project Introduction:

This comprehensive full-stack web application, crafted with React, Node.js, and PostgreSQL, efficiently manages customer data. Boasting a user-friendly interface, it showcases 50 dummy records in a paginated table, complete with search and sort functionalities. The inclusion of "date" and "time" columns enhances timestamp visibility, ensuring a seamless experience for exploring and managing customer information.

Let's delve into the step-by-step guide:

Step 1: Set up the Node.js Server

Navigate to the project folder in the command line:

bash
Copy code
cd project-folder
npm init -y
Install the necessary packages:

bash
Copy code
npm install express pg cors
Now, set up your server in the server.js file. Replace the existing code with your custom configuration:

javascript
Copy code
const pool = new Pool({
  user: 'your_username',
  host: 'localhost',
  database: 'your_database',
  password: 'your_password',
  port: 5432,
});
Remember to substitute the placeholder values with your PostgreSQL credentials.

Step 2: Set up PostgreSQL Database

Utilize the queries in the table.sql file to create the required table and the insertion.sql file for inserting data into the table.

Step 3: Set up the React App

Create a React app:

bash
Copy code
npx create-react-app your-react-folder-name
cd your-react-folder-name
Install the required packages:

bash
Copy code
npm install axios
Step 4: Replace the App.js Code

Replace the existing code in App.js with your custom code.

Step 5: Running

Open the Node.js command prompt, change the directory to the server folder, and execute the command:

bash
Copy code
node server.js
Once you see the message "Connected to port 3001," you've successfully connected to the server.

Now, in the Node.js command prompt, change the directory to your React app folder and run:

bash
Copy code
npm start
Congratulations! You have now successfully executed the application.
