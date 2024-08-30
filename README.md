# Library_Management_System

# Description:
This repository contains a Spring Boot-based Book Management System that provides RESTful APIs for managing book records in a library. The system allows users to perform CRUD operations on books, including adding, retrieving, updating, and deleting books. It utilizes a centralized logging mechanism to track and record API operations, ensuring transparency and easier debugging.

# Key Points:
* CRUD Operations: Implements Create, Read, Update, and Delete operations for book entities via RESTful endpoints.
* Logging: Uses SLF4J with Logback for logging key actions such as fetching, adding, updating, and deleting books, providing detailed operational logs.
* Repository Integration: Connects to a BookRepository that interacts with the database to persist and retrieve book records.
* Response Handling: Utilizes ResponseEntity to provide appropriate HTTP status codes and responses, ensuring clear communication of operation results.
* Error Handling: Includes basic error handling for scenarios where a book is not found, returning 404 Not Found for missing resources.
* Path Variable Usage: Extracts book IDs from URL paths to identify specific book records for retrieval, update, or deletion.

# Project Structure
librarymanagement ├── src │ ├── main │ │ ├── java │ │ │ └── com.example.librarymanagement │ │ │ ├── LibrarymanagementApplication.java │ │ │ ├── controller │ │ │ │ ├── BookController.java │ │ │ │ └── HomeController.java │ │ │ ├── model │ │ │ │ └── Book.java │ │ │ └── repository │ │ │ └── BookRepository.java │ ├── resources │ │ ├── static │ │ │ └── index.html │ │ └── templates │ │ └── application.properties ├── target │ ├── generated-sources/annotations │ ├── generated-test-sources/test-annotations ├── .mvn ├── .vscode ├── .gitignore ├── HELP.md ├── mvnw ├── mvnw.cmd └── pom.xml

Technologies Used
* Spring Boot
* Spring Data JPA
* Java 17
* Maven

# To Run:
Clone the repository:
```bash
 git clone https://github.com/meena-sharma/Library_Management_System
cd librarymanagementsystem 
```

Open the project in Visual Studio Code.

2.Run the project:

Use the built-in Spring Boot features to run the application directly from the IDE.

3.Access the application:

The REST API will be available at `(http://localhost:8081/)`. The home page can be accessed at `(http://localhost:8081/index.html)`.

# Screenshots:
Create Operation:
![lib post](https://github.com/user-attachments/assets/c640dbd3-012c-4660-b419-b0067c54e234)

Read Operation:
![lib get 2](https://github.com/user-attachments/assets/93d4f70d-2e7f-463e-9e13-7c40dbb0495a)

By id:
![lib 2 get](https://github.com/user-attachments/assets/5cf2cdc0-31e1-4795-ab03-b8354c6439e1)

Update Operation:
![lib put](https://github.com/user-attachments/assets/e9a52b15-3863-4031-b95a-06cbdb60c34d)

Delete Operation:
![lib delete](https://github.com/user-attachments/assets/0fa918f9-5eb8-4f99-8ea9-4d08f122a382)

![lib delete 2](https://github.com/user-attachments/assets/ef70bab8-ec71-4b67-bc3e-21c12ef90259)


