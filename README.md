To-Do List Application
This is a simple To-Do List Web Application developed using Spring Boot, Java, and Thymeleaf. It allows users to add tasks to a to-do list and view them.

Features
Add new tasks to the to-do list.
View all tasks in a clean and simple interface.

Technologies Used
Backend: Spring Boot (Java)
Frontend:HTML
Thymeleaf (for dynamic templates)
Build Tool: Maven
Server: Embedded Apache Tomcat (Spring Boot Default)

How to Run the Project Locally
Follow these steps to run the application on your local machine:

Clone the Project
Use Git to clone the repository:

git clone https://github.com/Ajay/Todoapp.git
cd Todoapp

Build the Application
Make sure you have Maven and Java 17+ installed. Run the following command:

mvn clean package
Run the Application
Run the generated JAR file:

java -jar target/Todoapp.jar
Access the Application
Open your browser and go to:
http://localhost:8080

Endpoints
HTTP Method	Endpoint	Description
GET	/	Show all tasks
POST	/add	Add a new task
How It Works
Users can add a task by entering a description and submitting the form.
The task will be displayed in the list below the input form.

Future Improvements
Add a "mark as completed" feature for tasks.
Persist tasks using a database (e.g., MySQL or H2).
Improve the user interface with CSS.

Contributors
Ajay Sharma







