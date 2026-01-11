# 🛒 E-Commerce Backend Project

A simple, robust REST API backend for an E-commerce application. Built with **Spring Boot** and **H2 Database**.

## 🚀 Tech Stack
* **Java** (Spring Boot)
* **Spring Data JPA** (Hibernate)
* **H2 Database** (In-memory database for instant testing)
* **Maven** (Build tool)

## 📂 Project Structure
This project follows the standard Layered Architecture:
* `Controller`: Handles HTTP requests.
* `Service`: Business logic.
* `Repository`: Database interaction.
* `Model`: Database entities.

## ⚙️ How to Run
You don't need to install a database! This project uses H2 (in-memory).

1.  **Clone the repo**
    ```bash
    git clone [https://github.com/surendraer/Ecom-project.git](https://github.com/surendraer/Ecom-project.git)
    cd Ecom-project
    ```

2.  **Run the App**
    * **Using Command Line:**
        ```bash
        ./mvnw spring-boot:run
        ```
    * **Using IDE (IntelliJ/Eclipse):**
        * Open the project.
        * Run `EcomProjectApplication.java`.

## 🔌 API Endpoints
(Use Postman or Browser to test these)

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/api/products` | Get all products |
| `GET` | `/api/product/{id}` | Get a single product by ID |
| `POST` | `/api/product` | Add a new product |
| `PUT` | `/api/product/{id}` | Update an existing product |
| `DELETE` | `/api/product/{id}` | Delete a product |

*(Note: If you get a 404 error, check if your methods inside ProductController.java use `/product` (singular) or `/products` (plural) and update this table accordingly).*

## 🗄️ H2 Database Console
You can view the database tables directly in your browser while the app is running.

1.  Go to: `http://localhost:8080/h2-console`
2.  **JDBC URL:** `jdbc:h2:mem:companydata`
3.  **User Name:** `sa`
4.  **Password:** (Leave Blank)
5.  Click **Connect**.

---
*Created by [Surendra](https://github.com/surendraer)*
