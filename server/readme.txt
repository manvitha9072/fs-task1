Classroom Management System
----------------------------
This is a simple Classroom Management System built using Node.js, Express, and MySQL. It allows teachers to create assignments, students to submit answers, and teachers to grade those submissions.

Features
--------
1. User Authentication: Users can log in with their username and password. Tokens are generated for authenticated users.
2. Assignment Creation: Teachers can create assignments specifying the name, description, subject, due date, class, and section.
3. Assignment Submission: Students can submit their answers for assignments.
4. Assignment Grading: Teachers can grade student submissions.
5. Email Reminders: Email reminders are sent to students for upcoming assignments.
6. Assignment Management: Teachers can delete assignments, and corresponding student answers will also be deleted.
7. Filtering Students: Teachers can filter students who have submitted a particular assignment before the due date.

Installation
------------
1. Clone this repository.
2. Install dependencies using npm install.
3. Set up MySQL database with the provided schema.
4. Update MySQL connection details in index.js.
5. Run the server using npm start.

Usage
-----
1. To log in, make a POST request to /login with your username and password.
2. Teachers can access protected routes like /teacher after logging in.
3. Create assignments by making a POST request to /create-assignment.
4. Students can submit answers using POST request to /submit-answer.
5. Teachers can grade submissions with a PUT request to /grade/:id.
6. Filter students who submitted an assignment before the due date by sending a POST request to /filter.