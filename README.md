# 🛍️ E-commerce Database Design

This project contains the full schema design for an e-commerce platform using MySQL. It includes an ERD, SQL schema, and a detailed breakdown of tables and relationships.

---

## 📦 Project Files

| File Name        | Description                                        |
|------------------|----------------------------------------------------|
| `ecommerce.sql`  | SQL file to create all tables in MySQL Workbench   |
| `erd.pdf`        | PDF export of the Entity Relationship Diagram      |

---

## 🛠️ Tools Used

- **MySQL Workbench** – for creating and managing the database
- **dbdiagram.io** – for visualizing and designing the ERD
- **VS Code / GitHub** – for version control and documentation

---

## 🧩 Tables Designed

1. `brand` – Brand information
2. `product_category` – Categories like clothing, electronics
3. `product` – General product details
4. `product_image` – Image URLs for each product
5. `color` – Available product color options
6. `size_category` – Groups of sizes (e.g., clothing sizes)
7. `size_option` – Specific size values (S, M, L, etc.)
8. `product_variation` – Links products to size and color combinations
9. `product_item` – Individual sellable items (with price & stock)
10. `attribute_type` – Types of attributes (text, number, boolean)
11. `attribute_category` – Categories of attributes (e.g., physical)
12. `product_attribute` – Custom attributes (e.g., material, weight)

---

## 🔁 Data Flow Explanation

The platform is structured in a way to support flexible and scalable product data. Here’s how the flow works:

1. **Brands** and **Categories** are created.
2. A **Product** is assigned to a Brand and a Category.
3. Each Product has **Images**, and optionally **Attributes** (e.g., material).
4. **Variations** of the Product are defined using **Color** and **Size Option**.
5. Each Variation becomes a **Product Item**, which has stock and price data.

---

## 🧮 ERD (Entity Relationship Diagram)

This project was initially modeled using **dbdiagram.io**. Below is the DBML code used to generate the ERD.

<details>
<summary>Click to view DBML code</summary>

