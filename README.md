# 🔄 MySQL REPLACE Statement Practice

## 📌 Project Overview
This practice project focuses on mastering the use of the **`REPLACE`** statement in MySQL, applied to realistic datasets from two different industries:  
- **Landscaping & Garden Design** (Lucky Shrub)  
- **Food & Beverage** (Little Lemon Mediterranean Restaurant)  

The `REPLACE` statement is a powerful MySQL command that allows you to insert new data or overwrite existing data based on primary or unique keys. It ensures that records are updated or replaced seamlessly without generating duplicate key errors.

---

## 🏢 Exercise 1 – Lucky Shrub (Landscaping & Garden Design)
**Industry Context:** Lucky Shrub is a medium-sized garden design firm that sells plants, landscaping materials, and decor.  
**Goal:** Manage and update customer orders efficiently.

### Sample Data – Before
| OrderID | ClientID | ProductID | Quantity | Cost   |
|---------|----------|-----------|----------|--------|
| 1       | Cl1      | P1        | 10       | 500.00 |
| 2       | Cl2      | P2        | 5        | 100.00 |
| 3       | Cl3      | P3        | 20       | 800.00 |
| 7       | Cl1      | P4        | 22       | 1200.00 |
| 8       | Cl1      | P1        | 15       | 150.00 |

### Actions Performed
- Added new orders for clients.
- Corrected an incorrect cost value for an existing order.
- Used primary key (`OrderID`) to target and replace specific rows.

### Sample Data – After
| OrderID | ClientID | ProductID | Quantity | Cost   |
|---------|----------|-----------|----------|--------|
| 1       | Cl1      | P1        | 10       | 500.00 |
| 2       | Cl2      | P2        | 5        | 100.00 |
| 3       | Cl3      | P3        | 20       | 800.00 |
| 7       | Cl1      | P4        | 22       | 1200.00 |
| 8       | Cl1      | P1        | 15       | 150.00 |
| 9       | Cl1      | P1        | 10       | 500.00 |
| 10      | Cl2      | P2        | 5        | 100.00 |

**What I Did:**
- Inserted new customer orders into the database.
- Corrected incorrect pricing data for an existing order.
- Practiced replacing records without creating duplicates by using primary keys as a reference.

**What I Achieved:**
- Learned how to use `REPLACE` to handle both **insertion** and **data correction** tasks.
- Simulated a real-world scenario where incorrect order details must be quickly corrected in a live database.

---

## 🍽 Exercise 2 – Little Lemon (Restaurant Industry)
**Industry Context:** Little Lemon is a family-owned Mediterranean restaurant specializing in traditional recipes with a modern twist.  
**Goal:** Manage menu items for the restaurant’s starter offerings.

### Sample Data – Before
| StarterName    | Cost | StarterType   |
|----------------|------|---------------|
| Cheese Bread   | 9.50 | Indian        |

### Actions Performed
- Added a new starter dish.
- Updated the cost of an existing dish.
- Maintained default category values while replacing details.

### Sample Data – After
| StarterName    | Cost | StarterType   |
|----------------|------|---------------|
| Cheese Bread   | 9.75 | Indian        |

**What I Did:**
- Added a new starter dish to the restaurant’s menu.
- Updated the cost of an existing dish without creating duplicate records.
- Maintained default category values while replacing item details.

**What I Achieved:**
- Practiced updating product details in a way that ensures menu accuracy.
- Simulated a real-world restaurant scenario where pricing changes need to be applied consistently.

---

## 🎯 Key Learning Outcomes
- Gained practical experience using the `REPLACE` statement in MySQL.
- Understood how `REPLACE` interacts with primary keys and unique constraints.
- Learned to apply `REPLACE` for both **data insertion** and **data correction** in industry-relevant scenarios.
- Enhanced database maintenance skills for **retail/order management** and **restaurant menu management**.
