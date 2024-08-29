Online Banking Application
Overview
The Online Banking Application is designed to enhance the customer experience in managing their bank accounts. It offers functionalities for both admin and customers, ensuring a seamless and secure banking experience.

Features
Admin Roles
Login: Admin can log in with a username and password.
Customer Registration: Register a customer with:
Full Name
Address
Mobile No
Email ID
Account Type (Savings or Current)
Initial Balance (minimum 1000)
Date of Birth
ID Proof

Generates an account number and a temporary password.
Customer Management: Add, delete, modify, and view customer details (excluding password and balance).
Customer Roles
Registration: Customers are registered by the admin and receive their account number and temporary password.
Login: Set up a new password using the account number and temporary password. Log in with the new password.
Logout: Customers can log out of their account.
Account Details: View account details and balance on the dashboard.
Transaction History: View the last 10 transactions in ascending or descending order of date.
Deposit: Deposit money to increase the balance, and the transaction is saved in the database.
Withdraw: Withdraw money to decrease the balance (balance cannot go below 0), and the transaction is saved in the database.
Account Closure: Close the account after withdrawing all the money.
Bonus: Download a PDF of the last 10 transactions.
Bill of Materials (BOM)
Eclipse IDE
Apache Tomcat 9
MySQL Server
MySQL Workbench
Java JDK (latest version)
JDBC Connector for MySQL
PDF Generation Library (e.g., iText)

Installation
Setup MySQL Database
Install MySQL Server and MySQL Workbench: Follow the installation instructions specific to your operating system.

Create Database:
Open MySQL Workbench and create a new database named banking.
Run the provided SQL script to create the necessary tables.

Configure Eclipse IDE
Install Eclipse IDE: Download and install Eclipse IDE from the official website.

Install Apache Tomcat 9 in Eclipse:
Go to Window > Preferences > Server > Runtime Environments.
Click Add, select Apache Tomcat 9, and follow the setup instructions.

Create a New Dynamic Web Project:
Go to File > New > Dynamic Web Project.
Enter the project name and configure the project settings.

Add Libraries
Add JDBC Connector:
Download the JDBC connector for MySQL and add it to the lib directory of your project.
Add PDF Generation Library:
Download the PDF generation library (e.g., iText) and add it to the lib directory of your project.
Deploy the Application
Write and Deploy:
Implement servlets, JSPs, and Java classes as required.
Configure the application to connect to the MySQL database using JDBC.
Deploy the application to the Apache Tomcat server.
Run the Application
Start Tomcat Server:
In Eclipse, go to the Servers view, right-click on the Tomcat server, and select Start.
Access the Application:
Open a web browser and navigate to the URL where your application is deployed (e.g., http://localhost:8080/your-app-name).
Database Schema
Tables
Admin

id (Primary Key)
username
password
Customer

id (Primary Key)
full_name
address
mobile_no
email_id
account_type (Savings/Current)
initial_balance
dob
id_proof
account_no
password
Transactions

id (Primary Key)
account_no
type (Deposit/Withdraw/Balance/Fund Transfer)
amount
date



![WhatsApp Image 2024-08-29 at 18 39 20_9924897c](https://github.com/user-attachments/assets/303d63cf-a0ec-48eb-b009-d5c5bbef5562)
![WhatsApp Image 2024-08-29 at 18 39 20_82ac4075](https://github.com/user-attachments/assets/e393e78c-de11-46a6-af16-2d87c7a4dbad)
![WhatsApp Image 2024-08-29 at 18 39 20_0b1d8a8c](https://github.com/user-attachments/assets/afbc07a5-5a53-4b3d-a7b3-932064df4f66)
![WhatsApp Image 2024-08-29 at 18 39 22_e9aa10f7](https://github.com/user-attachments/assets/2fb7a880-9bb5-45ea-bd46-36df03dc6cdc)
![WhatsApp Image 2024-08-29 at 18 39 22_818d4302](https://github.com/user-attachments/assets/73ecae42-a10a-435d-8111-ac4cb8a73612)
![WhatsApp Image 2024-08-29 at 18 39 21_25572498](https://github.com/user-attachments/assets/91944f70-ce26-4e06-9262-526c3b9e8202)
![WhatsApp Image 2024-08-29 at 18 39 21_24c9a9b6](https://github.com/user-attachments/assets/ddb880cb-8b4f-4293-9638-018066b8de93)
![WhatsApp Image 2024-08-29 at 18 39 21_3c1c58a4](https://github.com/user-attachments/assets/af8a6274-e72e-43b6-8159-00a8ce54beed)
![WhatsApp Image 2024-08-29 at 18 39 20_f0e7aae6](https://github.com/user-attachments/assets/43c5864e-2ae8-471b-aa3e-2575ef85fdf3)
![WhatsApp Image 2024-08-29 at 18 39 20_d211c08c](https://github.com/user-attachments/assets/3da9db3d-d705-42f2-8593-b01b9d4e7046)

