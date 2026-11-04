# 🍽️ Restaurant Billing System

A **menu-driven restaurant billing system** written in **C++** as the Second Semester Object-Oriented Programming project. Staff can take orders, edit or delete them, view all orders and print an itemised bill, and every change is saved to a text file.

![C++](https://img.shields.io/badge/C%2B%2B-00599C?logo=cplusplus&logoColor=white)
![OOP](https://img.shields.io/badge/Concept-OOP-blue)
![Interface](https://img.shields.io/badge/Interface-Console-lightgrey)
![Type](https://img.shields.io/badge/Type-Academic%20Project-lightgrey)

---

## 📑 Table of Contents

- [Features](#-features)
- [How It Works](#-how-it-works)
- [Quick Start](#-quick-start)
- [How to Use](#-how-to-use)
- [Menu](#-menu)
- [File Output Format](#-file-output-format)
- [Repository Contents](#-repository-contents)
- [Important Notes](#-important-notes)
- [Concepts Used](#-concepts-used)
- [Author](#-author)

---

## ✨ Features

- ➕ Add a customer order with any number of items
- 📝 Edit an existing order by adding more items
- ❌ Delete an order
- 📋 View all current orders with their totals
- 🧾 Generate an itemised bill for one order
- 📂 Orders are saved to `orders.txt` after every change
- 🍔 Fixed menu of 20 items (momos, burgers, pizzas, ice cream, drinks, sides, desserts)

---

## 🧩 How It Works

The program is built from three classes.

| Class | Role |
|-------|------|
| **MenuItem** | Holds an item's name and price |
| **Order** | Holds the customer name, table number, up to 50 items with quantities, and calculates the total |
| **Restaurant** | Manages up to 50 orders and provides add, edit, delete, view, bill and save |

```text
MenuItem ──► Order (items + quantities) ──► Restaurant (orders) ──► orders.txt
```

---

## ⚡ Quick Start

1. Install a C++ compiler such as `g++`.
2. Compile the program:

   ```bash
   g++ Final_Project.cpp -o Final_Project
   ```

3. Run it:

   ```bash
   ./Final_Project          # Windows: Final_Project.exe
   ```

4. Choose an option from the main menu.

---

## 📋 How to Use

The main menu looks like this:

```text
1. Add Order
2. Edit Order
3. Delete Order
4. View Orders
5. Generate Bill
6. Exit
Enter your choice:
```

| Option | What to do |
|--------|------------|
| **1. Add Order** | Enter the customer name (one word) and table number, then pick items by number with a quantity. Enter `1` to add another item or `0` to finish |
| **2. Edit Order** | Enter the order number, then add more items the same way |
| **3. Delete Order** | Enter the order number to remove it |
| **4. View Orders** | Shows every order with its items and total |
| **5. Generate Bill** | Enter the order number to print its itemised bill |
| **6. Exit** | Closes the program |

---

## 🍔 Menu

| No. | Item | Price (Rs.) | No. | Item | Price (Rs.) |
|-----|------|-------------|-----|------|-------------|
| 1 | Chicken Momo | 220 | 11 | Chocolate Ice Cream | 240 |
| 2 | Veg Momo | 180 | 12 | Strawberry Ice Cream | 240 |
| 3 | Paneer Momo | 250 | 13 | Coke | 80 |
| 4 | Ham Burger | 340 | 14 | Lemonade | 100 |
| 5 | Veg Burger | 200 | 15 | Iced Tea | 120 |
| 6 | Chicken Burger | 280 | 16 | French Fries | 150 |
| 7 | Pepperoni Pizza | 720 | 17 | Onion Rings | 180 |
| 8 | Veg Pizza | 620 | 18 | Garlic Bread | 200 |
| 9 | Chicken Pizza | 680 | 19 | Chocolate Cake | 300 |
| 10 | Vanilla Ice Cream | 240 | 20 | Brownie | 280 |

---

## 📄 File Output Format

Orders are written to `orders.txt`, one line per order:

```text
CustomerName,TableNo,Item1,Qty1,Item2,Qty2,...,TotalPrice
```

Example:

```text
Siddharth,2,French Fries,3,Paneer Momo,7,2200
```

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `Final_Project.cpp` | Source code |
| `Final_Project.exe` | Compiled Windows program |
| `orders.txt` | Saved orders (sample data) |
| `README.md` | Project documentation |

---

## 📝 Important Notes

- Orders are **saved but not loaded back** when the program starts, so a new run begins with an empty list and the first save overwrites `orders.txt`.
- The customer name is read with `cin >>`, so it must be a single word with no spaces.
- Editing an order only **adds** items; it cannot remove or change existing ones.
- The program holds at most 50 orders, and each order at most 50 items.
- An item number outside 1 to 20 is added as "Unknown" with a price of 0.

---

## 🧠 Concepts Used

- Classes and objects
- Encapsulation (private members in `Restaurant`)
- Constructors and member functions
- Arrays and strings
- File handling with `ofstream`
- Switch-case and loops

---

## 👤 Author

**Siddharth Acharya**
B.E. Computer Engineering, Himalaya College of Engineering (HCOE), Tribhuvan University
Second Semester OOP Project
GitHub: [@acharya-2226](https://github.com/acharya-2226)

Open for educational and personal use. Feel free to adapt it for your own learning.
