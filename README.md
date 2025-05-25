# AgriConnect - Java GUI Crop Price Calculator with MySQL

AgriConnect is a simple Java-based desktop application that allows users (especially farmers or market agents) to calculate crop prices, enter quantities, and store sales data into a MySQL database using JDBC. This project was developed for an academic GUI-based project submission and includes all necessary components like MVC architecture, database connectivity, and responsive GUI.

---

## Features

- GUI built with **Java Swing**
- 5 crops with pre-set price per kg
- User inputs quantity and sees the total price
- Sales data is **saved to MySQL** via **JDBC**
- Modular code using **Model, DAO, and Controller design pattern**
- Aesthetic and responsive layout

---

## Technologies Used

- Java (JDK 8+)
- Java Swing (GUI)
- JDBC (MySQL Connector)
- MySQL Database

---

## Crop Pricing Table

| Crop       | Price per Kg (Rs.) |
|------------|--------------------|
| Wheat      | 25.50              |
| Rice       | 32.00              |
| Maize      | 28.00              |
| Sugarcane  | 30.50              |
| Millet     | 27.50              |

---

## Project Structure

```
AgriConnect/
├── AgriConnectMain.java     # GUI + Controller
├── Crop.java                # Model class
├── CropDAO.java             # DAO for MySQL
└── DBConnection.java        # JDBC utility
```

---

## MySQL Setup

```sql


CREATE TABLE IF NOT EXISTS crop_sales (
    id INT AUTO_INCREMENT PRIMARY KEY,
    crop_name VARCHAR(50),
    quantity INT,
    price DOUBLE,
    total DOUBLE,
    sale_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

---




## Review 1 Rubric Checklist

| Deliverable Title                                         | Status |
|-----------------------------------------------------------|--------|
| JDK & IDE Setup                                           | ✅     |
| Project Structure Defined                                 | ✅     |
| Database Schema Designed                                  | ✅     |
| MySQL Table Created                                       | ✅     |
| JDBC Connectivity Implemented                             | ✅     |
| Model, DAO Classes Created                                | ✅     |
| Aesthetics and Visual Appeal of UI                        | ✅     |
| Component Placement and Alignment                         | ✅     |
| Responsiveness and Accessibility of UI                    | ✅     |

---

## Author

**Team Nandighosh **
B.Tech CSE, Galgotias University  


---

## License

This project is licensed under the MIT License.
