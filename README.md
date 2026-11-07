# Periodic Table Database 🧪

A relational database and Bash-scripting project built to manage chemical elements data and query it dynamically, completed as part of the FreeCodeCamp Relational Database certification.

## 📋 Features
- **Relational Database (`periodic_table`)**: Structured using `elements`, `properties`, and `types` tables with proper foreign key constraints, `UNIQUE`, and `NOT NULL` validations.
- **Data Normalization**: Cleaned data, removed trailing zeros from atomic masses using `REAL` data types, and capitalized chemical symbols properly using `INITCAP()`.
- **Bash Script (`element.sh`)**: An interactive command-line tool that retrieves element details (Atomic Number, Name, Symbol, Type, Atomic Mass, Melting Point, and Boiling Point) using either the atomic number, symbol, or full name.
- **Git Version Control**: Maintained with a clean commit history following conventional commit message standards (`feat:`, `chore:`, `Initial commit`).

---

## 🛠️ Database Schema
- **`elements`**: Stores `atomic_number` (Primary Key), `symbol` (Unique, Not Null), and `name` (Unique, Not Null).
- **`types`**: Stores `type_id` (Primary Key) and `type` (e.g., metal, nonmetal, metalloid).
- **`properties`**: Stores `atomic_number` (Foreign Key), `atomic_mass`, `melting_point_celsius`, `boiling_point_celsius`, and `type_id` (Foreign Key).

---

## 🚀 How to Run the Script

1. Clone the repository and navigate to the project folder:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/periodic-table.git](https://github.com/YOUR_USERNAME/periodic-table.git)
   cd periodic-table
