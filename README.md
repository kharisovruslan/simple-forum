# Simple Forum

## 📝 Description
Simple Forum is a lightweight web application built using the Spring Framework. It allows users to create topics, post replies, browse discussions, and manage content with built-in role-based access control.

## 🛠️ Technologies
* **Backend:**
  * **Java 21** (including modern features like Optionals and Streams)
  * **Spring Boot 2.7.x** (automatic configuration and deployment)
  * **Spring MVC** (clean architecture based on the Model-View-Controller pattern)
  * **Spring Data JPA & Hibernate** (relational mapping, custom JPQL, and native queries)
  * **Spring Security** (custom login/registration forms, database-backed authentication, and role-based authorization)
  * **Lombok** (boilerplate code reduction)

* **Database:**
  * **H2 Database** (in-memory database used for fast development and testing)
  * **Apache Derby** (embedded SQL database support)

* **Frontend:**
  * **HTML5 & Thymeleaf** (server-side template engine with secure SpEL expressions)
  * **CSS3 & Bootstrap** (responsive and clean user interface)
  * **JavaScript & jQuery** (client-side interactive elements)

## 🚀 Key Features
* **Topic Management:** Users can browse existing topics and create new discussion threads.
* **Message System:** Interactive commenting within topics, support for line breaks, and content rendering.
* **Security & Roles:** 
  * Registration with encrypted passwords using `PasswordEncoder`.
  * Multi-role system (`ROLE_USER` for regular members, `ROLE_ADMIN` for content moderation).
  * Administrative capability to delete messages directly from the UI.
* **Data Validation:** Server-side forms validation using `spring-boot-starter-validation` (constraints like `@NotBlank`, `@Size`, etc.).

## ⚙️ How to Run

### Prerequisites
* Java Development Kit (JDK) 21 or higher
* Apache Maven 3.x

### Steps
1. **Clone the repository:**
   ```bash
   git clone https://github.com/kharisovruslan/simple-forum
   cd simple-forum
   ```

2. **Build the project:**
   ```bash
   mvn clean package
   ```

3. **Run the application:**
   ```bash
   mvn spring-boot:run
   ```
4. Open your browser and navigate to `http://localhost:8080`.