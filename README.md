# Hospital-Management-System
The Hospital Management System is a comprehensive solution for managing hospital operations efficiently. It features patient registration, appointment scheduling, doctor and staff management, medical records, billing, and inventory management. Built with a robust backend using Java servlets and MySQL, it ensures seamless data handling and security.


# Hospital Management System

Welcome to the Hospital Management System project! This README file provides an overview of the project, including installation instructions, features, and other essential details.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Requirements](#requirements)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Project Structure](#project-structure)
7. [Contributing](#contributing)

## Introduction

The Hospital Management System is a comprehensive web application designed to manage hospital operations efficiently. It includes patient registration, appointment scheduling, doctor and staff management, medical records, billing, and inventory management. The system is built using Java Servlets for the backend, with HTML, CSS, and JavaScript for the frontend.

## Features

- **Patient Management**: Register and manage patient details.
- **Appointment Scheduling**: Schedule and manage patient appointments.
- **Doctor Management**: Manage doctor details and schedules.
- **Medical Records**: Maintain patient medical history and records.
- **Billing System**: Generate and manage patient bills.
- **Inventory Management**: Track and manage hospital inventory and supplies.
- **User Authentication**: Secure login and user management.

## Requirements

- **Java Development Kit (JDK)**: Version 8 or later
- **Apache Tomcat**: Version 9 or later
- **MySQL**: Version 5.7 or later
- **Maven**: Version 3.6 or later
- **Web Browser**: Latest version of Chrome, Firefox, or Edge

## Installation

### Backend Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Bhushanseelan/Hospital-Management-System.git
   cd Hospital-Management-System
   ```

2. **Set Up MySQL Database**:
   - Create a new MySQL database:
     ```sql
     CREATE DATABASE hospital_management;
     ```
   - Import the database schema and sample data from `db/hospital_management.sql`:
     ```bash
     mysql -u root -p hospital_management < db/hospital_management.sql
     ```

3. **Configure Database Connection**:
   - Update the database connection details in `src/main/resources/db.properties`.

4. **Build the Project**:
   ```bash
   mvn clean install
   ```

5. **Deploy to Tomcat**:
   - Copy the generated WAR file from `target/hospital-management-system.war` to the `webapps` directory of your Tomcat server.
   - Start the Tomcat server.

### Frontend Setup

1. **Navigate to the Project Directory**:
   ```bash
   cd Hospital-Management-System
   ```

2. **Open the Project in Your Preferred IDE**.

3. **Access the Application**:
   - Open your web browser and navigate to `http://localhost:8080/hospital-management-system`.

## Usage

1. **Login**:
   - Access the login page and enter your credentials.
   - Admin credentials can be found in the sample data imported into the database.

2. **Dashboard**:
   - After logging in, you will be redirected to the dashboard where you can manage patients, doctors, appointments, billing, and inventory.

3. **Patient Management**:
   - Register new patients, update existing patient details, and view patient medical records.

4. **Appointment Scheduling**:
   - Schedule new appointments, update existing appointments, and view appointment details.

5. **Doctor Management**:
   - Add new doctors, update doctor details, and manage doctor schedules.

6. **Billing System**:
   - Generate new bills, update existing bills, and view billing history.

7. **Inventory Management**:
   - Track and manage hospital inventory and supplies.

## Project Structure

```
Hospital-Management-System/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/hospital/
│   │   │       ├── controller/
│   │   │       ├── dao/
│   │   │       ├── model/
│   │   │       └── service/
│   │   ├── resources/
│   │   │   └── db.properties
│   │   └── webapp/
│   │       ├── css/
│   │       ├── js/
│   │       └── WEB-INF/
│   │           ├── web.xml
│   │           └── views/
│   └── test/
├── db/
│   └── hospital_management.sql
├── pom.xml
└── README.md
```

## Contributing

We welcome contributions to the Hospital Management System! If you have any ideas, bug fixes, or enhancements, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Create a new Pull Request.

