![GitHub repo size](https://img.shields.io/github/repo-size/shivamkachhadiya/Bloging_Project_SpringBoot)
![Project Type](https://img.shields.io/badge/project-Blogging_App-green)
![Tech Stack](https://img.shields.io/badge/built%20with-SpringBoot%20%7C%20Java%20%7C%20HTML-orange)
![Top Language](https://img.shields.io/github/languages/top/shivamkachhadiya/Bloging_Project_SpringBoot)
![Location](https://img.shields.io/badge/location-VIT_Vellore-9cf)
![Goal](https://img.shields.io/badge/goal-Fintech_PBC-orange)
![TimeZone](https://img.shields.io/badge/timezone-IST-blue)
![Profile Views](https://komarev.com/ghpvc/?username=shivamkachhadiya)

📝 BloggingProject

A simple blogging platform built using **Spring Boot**, with **MySQL** as the backend database and **IntelliJ IDEA** as the development environment.

**1) Home Page Of Project (Blogging)**

![image](https://github.com/user-attachments/assets/ecee7bfd-e341-466c-825e-82dd1b33d8c8)

**2) New Page For Adding Ideas & Thoughts**

![image](https://github.com/user-attachments/assets/6a19447e-6d99-4c91-9857-0b11949685d9)

**3) Update Page For Updating Ideas In Future**
![image](https://github.com/user-attachments/assets/6f22f13b-a0d0-4260-8a99-844f4048b82e)

**4) Delete Works Whenever You Click On Delete Button**



---

## 📦 Tech Stack

- **Backend**: Java, Spring Boot, Spring Data JPA
- **Database**: MySQL (managed using MySQL Workbench)
- **ORM**: Hibernate (JPA)
- **IDE**: IntelliJ IDEA
- **Build Tool**: Maven

---

## 🚀 Features

- Create and manage blog posts
- Store post data in a MySQL database
- Automatically map Java classes to database tables using Hibernate
- REST-ready structure (easy to extend to APIs)

---

## 📁 Project Structure
```
BloggingProject/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/
│       │       └── blog/
│       │           └── BlogingProject/
│       │               ├── model/
│       │               │   └── Post.java
│       │               ├── repository/
│       │               │   └── PostRepository.java
│       │               └── BloggingProjectApplication.java
│       └── resources/
│           └── application.properties
└── pom.xml
```


---

## 🧠 How It Works

1. `Post` class is annotated with `@Entity` and mapped to a `post` table.
2. Spring Boot reads `application.properties` to configure database connection.
3. On startup, Hibernate creates the necessary table if not present.
4. Repositories enable CRUD operations on the `post` table.

---

## ⚙️ Configuration

### 🔑 application.properties

```properties```
spring.application.name=BloggingProject
spring.datasource.url=jdbc:mysql://127.0.0.1:3306/blogpost
spring.datasource.username=root
spring.datasource.password=Latif#@123
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
spring.jpa.hibernate.ddl-auto=update

# Optional for debugging
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true


🛠 Setup Instructions
1. Clone the repository
2. git clone https://github.com/your-username/BloggingProject.git
cd BloggingProject
3. Create MySQL database
   CREATE DATABASE blogpost;
4. Open in IntelliJ IDEA
   Import project as Maven project
   Wait for dependencies to resolve
5. Run the project
   Run BloggingProjectApplication.java

📄 License
This project is open source. Feel free to use and modify.
