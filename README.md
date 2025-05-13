# Ex09 Event Registration Web Application
## Date:13-05-2025
# NAME : MOHAMED HAFEEZ S
# REG NO : 212224040193
## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
HTML 
<!DOCTYPE html>
<html>
<head><title>Register</title></head>
<body>
  <h2>Event Registration</h2>
  <form action="/register" method="POST">
    <input name="name" placeholder="Name" required>
    <input name="email" placeholder="Email" required>
    <button>Submit</button>
  </form>
</body>
</html>

JAVASCRIPT 
const express = require('express');
const app = express();
const port = 3000;
let registrations = [];

app.use(express.urlencoded({ extended: true }));
app.use(express.static('public'));

app.post('/register', (req, res) => {
  registrations.push(req.body);
  res.send(`<h3>Thanks, ${req.body.name}!</h3><a href="/">Back</a>`);
});

app.listen(port, () => console.log(`Running on http://localhost:${port}`));
## OUTPUT:
![Screenshot 2025-05-13 142409](https://github.com/user-attachments/assets/5389e598-486e-41c3-bac1-cf9e4ffc0d08)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
