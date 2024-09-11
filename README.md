# ContactAPI - Spring Boot CRUD Application

This repository contains the backend code for a Contact API developed using Java and Spring Boot. It allows users to perform CRUD (Create, Read, Update, Delete) operations on contacts and attach pictures to each contact. The project also includes integration for uploading and retrieving images.

## Features

- **CRUD Operations**: Create, Read, Update, Delete contacts.
- **Image Upload**: Attach and retrieve profile pictures for each contact.
- **REST API**: Fully implemented REST API for managing contacts.
- **Database**: Integrated with PostgreSQL/MySQL for data persistence.
- **MultipartFile Handling**: Supports file uploads using `MultipartFile`.

## Technologies Used

- **Backend**: Java, Spring Boot
- **Database**: PostgreSQL/MySQL
- **ORM**: Hibernate/JPA
- **Image Handling**: `MultipartFile`
- **Build Tool**: Maven
- **API Testing**: Postman, JUnit (optional)

## Getting Started

### Prerequisites

- Java 17+
- Maven
- PostgreSQL/MySQL database
- IDE of your choice (IntelliJ IDEA, Eclipse, etc.)

### Setup and Running Locally

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/contactapi.git
    cd contactapi
    ```

2. **Configure Database:**
   - Update your `application.properties` or `application.yml` with the appropriate database configurations:
     ```properties
     spring.datasource.url=jdbc:postgresql://localhost:5432/your-database-name
     spring.datasource.username=your-username
     spring.datasource.password=your-password
     spring.jpa.hibernate.ddl-auto=update
     ```

3. **Run the Application:**
    ```bash
    mvn spring-boot:run
    ```

4. **Access the API:**
   The API will be accessible at `http://localhost:8080/api/contacts`.

### API Endpoints

- **GET /api/contacts** - Retrieve all contacts.
- **GET /api/contacts/{id}** - Retrieve a specific contact by ID.
- **POST /api/contacts** - Create a new contact (supports image upload).
- **PUT /api/contacts/{id}** - Update an existing contact by ID.
- **DELETE /api/contacts/{id}** - Delete a contact by ID.

### Sample API Request (Create Contact)

To create a new contact with an image, send a `POST` request to `/api/contacts` with form-data:

| Key         | Value          |
|-------------|----------------|
| name        | John Doe       |
| email       | john@example.com|
| phone       | 1234567890     |
| image       | [upload image] |

### Frontend Integration

This API is designed to work with any frontend. You can easily integrate it with a React, Angular, or Vue.js frontend, or use the provided frontend repository here:

- [Frontend GitHub Repo](https://github.com/Jonathan-Tong1/contactapp-main)

### Deployment

You can deploy the API to any cloud provider or platform that supports Java applications, such as:

- **Heroku**
- **AWS EC2**
- **Google Cloud**
- **Docker**

Make sure to adjust the database configuration according to your deployment environment.

### License

This project is **not licensed**. You may use or modify the code as you see fit, but there is no official license attached.

### Contact

For any questions or inquiries, feel free to reach out to **jontong321@gmail.com**.

---

This version includes your contact information and reflects that the project is not officially licensed. Let me know if you'd like to adjust anything further!
