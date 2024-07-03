# Validations

## Overview

The `Validations` project is a Java application that demonstrates user data management with Jakarta Bean Validation and Hibernate ORM. This project includes features for validating user data and saving it to a MySQL database.

## Features

- **User Data Management:** Collect and validate user details.
- **Data Validation:** Utilize Jakarta Bean Validation for data integrity.
- **Database Interaction:** Persist validated user data to a MySQL database using Hibernate.

## Prerequisites

To run this project, you will need:

- **Java JDK 11+**: [Download JDK](https://www.oracle.com/java/technologies/javase-downloads.html)
- **Maven**: [Download Maven](https://maven.apache.org/download.cgi)
- **MySQL Database**: [Download MySQL](https://dev.mysql.com/downloads/mysql/)
- **Git**: [Download Git](https://git-scm.com/downloads)

## Installation

Follow these steps to set up the project:

1. **Clone the Repository**

   Open your terminal or command prompt and run:

   ```sh
   git clone https://github.com/BevinIseac/Validations.git
   cd Validations
   
Install Dependencies

Use Maven to install the required dependencies:


mvn install
Configure the Database

Update hibernate.cfg.xml with your MySQL credentials. You can find this file in the src/main/resources directory. Replace the placeholders with your actual database credentials:


<hibernate-configuration>
    <session-factory>
        <property name="hibernate.connection.driver_class">com.mysql.cj.jdbc.Driver</property>
        <property name="hibernate.connection.url">jdbc:mysql://localhost:3306/your_database_name</property>
        <property name="hibernate.connection.username">your_username</property>
        <property name="hibernate.connection.password">your_password</property>
        <property name="hibernate.dialect">org.hibernate.dialect.MySQLDialect</property>
        <property name="hibernate.current_session_context_class">thread</property>
        <property name="hibernate.show_sql">true</property>
        <property name="hibernate.hbm2ddl.auto">update</property>
    </session-factory>
</hibernate-configuration>
Run the Application

Start the application with the following Maven command:


mvn exec:java -Dexec.mainClass="com.java.Test"
Usage
Launch the Application: Run the Test class to start the application.
Enter User Details: Follow the prompts to input user information. Valid data will be saved to the database.
Contributing
If you want to contribute to this project:

Fork the Repository: Click the "Fork" button on the GitHub page to create your own copy of the repository.

Create a Branch: Create a new branch for your changes:

git checkout -b new-feature
Make Changes: Edit the code or documentation as needed.

Commit Changes: Commit your changes with a descriptive message:


git commit -am 'Add new feature'
Push Changes: Push your changes to your forked repository:


git push origin new-feature
Create a Pull Request: Go to your forked repository on GitHub and click the "Compare & pull request" button.
