# 📚 Course Service (Spring Boot + GCP MySQL)

A **Spring Boot application** for managing course data, backed by a **MySQL database** hosted on **Google Cloud SQL**.  
The project leverages **Spring Profiles** (`local`, `gcp`) to seamlessly switch between local development and cloud deployment.

---

## 🚀 Demo on GCP
🎥 [Watch the Demo Video](https://drive.google.com/file/d/1TIt2MHD6NvnaeV7orNlNHk-Pa2PqWT8p/view?usp=sharing)

---

## 🛠️ Prerequisites

- **Java 21 (LTS)**
- **Spring Boot 3+**
- **MySQL Database** (Local or GCP Cloud SQL)
- **Google Cloud SQL Instance** (for cloud profile)
- **Maven/Gradle** (for build and dependency management)

---

## ⚙️ Database Configuration

### 🔹 Local Profile (`application-local.properties`)
Use this when running locally with a MySQL instance:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/course_db?createDatabaseIfNotExist=true&useSSL=false&allowPublicKeyRetrieval=true
spring.datasource.username=root
spring.datasource.password=your_local_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
