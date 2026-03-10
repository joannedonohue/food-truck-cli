# 🚚 Food Truck CLI

> An interactive, terminal-based ordering system for a multi-cuisine food truck — built in pure Python.

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

---

## Overview

Food Truck CLI is a command-line point-of-sale application that simulates a real-world ordering experience. Customers browse a multi-category menu, choose items with variants and sizes, specify quantities, and receive a formatted receipt with a running total — all from the terminal.

The project demonstrates practical Python fundamentals: nested data structures, control flow, user input validation, list comprehension, and formatted string output.

---

## Features

- **Multi-category menu** — Snacks, Meals, Drinks, and Dessert
- **Nested item variants** — Handles sub-items like `Pizza - Pepperoni` and `Soda - Large`
- **Robust input validation** — Gracefully handles non-numeric and out-of-range entries, defaulting where appropriate
- **Multi-item ordering** — Customers can add items across categories in a single session
- **Formatted receipt** — Tabular order summary with aligned columns for item name, price, and quantity
- **Order total** — Calculated via list comprehension across the full order

---

## Demo

```
Welcome to the variety food truck.

From which menu would you like to order?
1: Snacks
2: Meals
3: Drinks
4: Dessert
Type menu number: 2

Item # | Item name                 | Price
-------|---------------------------|-------
1      | Burrito                   | $4.49
2      | Teriyaki Chicken          | $9.99
3      | Sushi                     | $7.49
4      | Pad Thai                  | $6.99
5      | Pizza - Cheese            | $8.99
6      | Pizza - Pepperoni         | $10.99
7      | Pizza - Vegetarian        | $9.99
8      | Burger - Chicken          | $7.49
9      | Burger - Beef             | $8.49

What Meals would you like to order? 1
How many Burrito would you like to order? 2

Would you like to keep ordering? (Y)es or (N)o: N
Thank you for your order. We are preparing your food now.

This is what we are preparing for you.

Item name                  | Price   | Quantity
---------------------------|---------|----------
Burrito                    | $4.49   | 2
Total cost: $8.98
```

---

## Getting Started

**Requirements:** Python 3.x — no external dependencies.

```bash
# Clone the repo
git clone https://github.com/joannedonohue/food-truck-cli.git
cd food-truck-cli

# Run the app
python menu.py
```

---

## Project Structure

```
food-truck-cli/
├── menu.py       # Menu data and full ordering logic
└── README.md
```

---

## Key Concepts

| Concept | Where Used |
|---|---|
| Nested dictionaries | Menu data structure (category → item → variant → price) |
| While loops + break | Order flow and input retry logic |
| Input validation | Numeric checks, range checks, quantity fallback |
| f-strings | Formatted table output with dynamic column spacing |
| List comprehension | Order total calculation |

---

## License

MIT
