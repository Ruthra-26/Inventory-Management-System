# Inventory Management System

A simple inventory management project with:
- HTML, CSS and JavaScript frontend
- Java Spring Boot REST API
- MySQL database

## Project structure

```text
inventory-management-github/
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── inventory.js
├── backend/
│   ├── pom.xml
│   └── src/main/
│       ├── java/com/inventory/inventory_management/
│       │   ├── InventoryManagementApplication.java
│       │   ├── Product.java
│       │   ├── ProductRepository.java
│       │   └── ProductController.java
│       └── resources/application.properties
└── database/
    └── inventory.sql
```

## Database setup
1. Open MySQL Workbench or your MySQL terminal.
2. Run `database/inventory.sql`.
3. Update the username and password in `backend/src/main/resources/application.properties`.

## Run the backend
Open a terminal in the `backend` folder and run:

```bash
mvn spring-boot:run
```

The API runs at `http://localhost:8080/api/products`.

## Run the frontend
Open `frontend/index.html` in a browser while the backend is running.

> The frontend uses the API at `http://localhost:8080/api/products`. For deployment, configure the API URL and CORS settings for your hosting setup.
