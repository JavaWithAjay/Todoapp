To-Do App
This is a simple To-Do application built with Java and Spring Boot. This application allows users to add and view tasks in a to-do list. It is deployed on AWS EC2, with a scalable architecture designed to handle increased traffic, ensuring better availability and performance.
•	Scalable Architecture: Designed and deployed a scalable architecture using AWS EC2 with load balancing and auto-scaling to handle varying traffic and ensure high availability.
•	Deployment on AWS EC2: The application is deployed on an EC2 instance, with public accessibility.
•	CloudWatch Monitoring: Integrated AWS CloudWatch to monitor the application's performance, including metrics like CPU utilization, disk I/O, and network traffic.
________________________________________
Features
•	Add new tasks to the to-do list.
•	View all added tasks.
________________________________________
Technologies Used
•	Java (Spring Boot)
•	Maven (for project management and dependencies)
•	AWS EC2 (for deployment)
•	AWS CloudWatch (for monitoring system metrics)
•	AWS Load Balancer and Auto-Scaling (for scalability)
•	AWS Security Groups (for security)
________________________________________
Getting Started Locally
Step 1: Clone the Repository
git clone https://github.com/JavaWithAjay/Todoapp.git 
cd Todoapp
Step 2: Install Java (JDK 17 or higher)
Make sure that Java 17 (or higher) is installed on your system. You can verify this by running:
java -version
If Java is not installed, download and install it from the Oracle Java Downloads page or use an OpenJDK distribution.
________________________________________
Step 3: Build the Application
Use Maven to build the application and create a JAR file:
mvn clean package
The built JAR file will be located in the target/ folder.
________________________________________
Step 4: Run the Application Locally
Run the application using the following command:
java -jar target/Todoapp.jar
The application will be available at http://localhost:8080.
________________________________________
Deploying on AWS EC2 (Windows)
Step 1: Launch an EC2 Instance
1.	Log in to the AWS Management Console and go to EC2 Dashboard.
2.	Launch a new Windows-based EC2 instance (e.g., using Windows Server 2019).
3.	Make sure to open port 8080 in the Security Group settings to allow access to the Spring Boot app.
________________________________________
Step 2: Install Java on EC2
Once connected to the EC2 instance, install Java (JDK 17 or higher):
1.	Download and install JDK 17 from the official Oracle site.
2.	Verify the installation:
java -version
________________________________________
Step 3: Upload the JAR File to EC2
You can use MobaXterm or WinSCP to upload the Todoapp.jar file from your local machine to your EC2 instance.
For MobaXterm:
•	Connect to your EC2 instance using MobaXterm with your EC2 credentials.
•	Upload the Todoapp.jar file to a directory on your EC2 instance (e.g., C:\Users\Administrator\).
________________________________________
Step 4: Run the Application on EC2
1.	Open Command Prompt or PowerShell on the EC2 instance.
2.	Navigate to the directory where the JAR file is uploaded.
3.	Run the Spring Boot application:
java -jar Todoapp.jar
The application will run on port 8080.
________________________________________
Step 5: Access the Application
Open your web browser and enter the Public IP address of the EC2 instance followed by :8080. Example:
http://3.110.123.29:8080 
You should now be able to access the Spring Boot To-Do app running on your AWS EC2 instance.
________________________________________
Scalable Architecture Setup
For this application, we have designed a scalable architecture that includes the following components:
1.	AWS EC2 Instances: Running the Spring Boot application.
2.	AWS Load Balancer: Distributes incoming traffic across multiple EC2 instances to ensure high availability and fault tolerance.
3.	Auto-Scaling: Automatically scales the number of EC2 instances based on the demand, ensuring the application can handle varying traffic loads.
4.	Elastic IP & Public Accessibility: EC2 instances are publicly accessible through an elastic IP, allowing global access to the app.
This scalable architecture ensures the application can handle increased traffic and remain available under varying load conditions.
![scale_page-0001](https://github.com/user-attachments/assets/d30fdf90-7a1f-4809-a44d-d4b07b1dddcf)
________________________________________
Monitoring Application Metrics Using AWS CloudWatch
To monitor the performance and health of the deployed To-Do app on AWS EC2, AWS CloudWatch has been configured.
Steps to Monitor Metrics:
1.	Log in to AWS Management Console.
2.	Go to EC2 Dashboard > Select your EC2 instance.
3.	Click on the Monitoring Tab.
4.	You can view the following system metrics:
o	CPU Utilization
o	Network In/Out
o	Disk Reads/Writes
 
_________![image](https://github.com/user-attachments/assets/2cd0b42b-36b1-40ba-b161-21c5f3df4530)
_______________________________
Future Improvements
•	User Authentication: Add a user login and registration system to allow users to securely manage their tasks.
•	Database Integration: Integrate a database (like MySQL or PostgreSQL) to store tasks persistently instead of in-memory storage.
•	Task Priority: Add the ability to set priorities or deadlines for tasks.
•	Task Categories: Organize tasks into different categories or tags for better management.
________________________________________
Conclusion
Your Spring Boot To-Do app is now live on AWS EC2 with a scalable architecture and is being monitored using AWS CloudWatch. This guide demonstrates how to:
1.	Deploy a web application on AWS EC2.
2.	Implement a scalable architecture with Load Balancing and Auto-Scaling.
3.	Monitor system metrics using CloudWatch.
You can access the app through the public URL provided by AWS:
http://<your-ec2-public-ip>:8080

