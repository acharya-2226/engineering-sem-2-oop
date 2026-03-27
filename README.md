# 🍽️ Restaurant Billing System (Second Semester OOP Project)

This is a **menu-driven Restaurant Billing System** developed in **C++** as part of the **Second Semester Object-Oriented Programming Project** for Computer Engineering. The system enables restaurant staff to manage **orders**, generate **bills**, and store order data using file handling. Core OOP concepts like encapsulation and modularity are demonstrated through classes such as `MenuItem`, `Order`, and `Restaurant`.

> 🎓 **Second Semester Computer Engineering Project**

---

## 🛠️ Features

- ➕ Add new customer orders (multiple items per order)
- 📝 Edit existing orders
- ❌ Delete orders
- 📋 View all current orders
- 🧾 Generate itemized bill for a specific order
- 📂 Orders saved to `orders.txt` for basic persistence

---

## 🧠 Concepts Used

- Classes and Objects
- Encapsulation
- Modular design
- File handling (`ofstream`, file writing)
- Arrays and Strings
- Switch-case and Loops

---

## 🍔 Menu Items

The menu features 20 items, including momos, burgers, pizzas, beverages, and desserts, each with a set price.

Example:

```
1. Chicken Momo - Rs.220
2. Veg Momo - Rs.180
...
20. Brownie - Rs.280
```

---

## ▶️ How to Run

### Requirements

- C++ compiler (e.g., g++)

### Compile

```bash
g++ restaurant_billing.cpp -o restaurant_billing
```

### Run

```bash
./restaurant_billing
```

---

## 📂 File Output Format

Orders are stored in `orders.txt` in the following format:

```
CustomerName,TableNo,Item1,Qty1,Item2,Qty2,...,TotalPrice
```

---

## 📋 Sample Menu

```
1. Add Order
2. Edit Order
3. Delete Order
4. View Orders
5. Generate Bill
6. Exit
Enter your choice:
```

---

## 📚 Educational Purpose

This project helps students:

- Apply object-oriented design to real-world systems
- Model entities (like `Order`, `MenuItem`) using classes
- Practice file handling and user interaction in console applications

---

## 👨‍💻 Author

- **Project by:** Siddharth
- **Semester:** Second
- **Program:** B.E. Computer Engineering

---

## 📜 License

This project is intended for academic and learning purposes. You may use, modify, and enhance it for coursework or personal projects.

---

## 🙏 Acknowledgments

Special thanks to faculty and classmates for their support and guidance during this project.

Folder update note: This directory name was updated and this README was touched to keep folder-level changes tracked in Git.
Small documentation refresh for commit traceability.
