# 💇 Salon Booking CLI

A command-line salon booking system built with **Bash** and **PostgreSQL**.

This project simulates a real-world appointment scheduling system for a beauty salon, allowing service selection, customer management, and appointment booking directly from the terminal.

---

## 🚀 Features

- 📋 List available salon services
- 👤 Register new customers
- 🔎 Search customers by phone number
- 📅 Create appointments
- 🗄 PostgreSQL relational database integration
- 🔁 Auto-increment ID handling with sequences
- 🧠 Structured business logic in Bash

---

## 🛠 Tech Stack

- **Bash (Shell Scripting)**
- **PostgreSQL**
- SQL (CRUD operations, sequences, constraints)

---

## 🗂 Database Structure

### Tables:

- `services`
- `customers`
- `appointments`

### Relationships:

- `appointments.customer_id` → references `customers.customer_id`
- `appointments.service_id` → references `services.service_id`

---

## ⚙️ How to Run

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Pedrolo626/salon-booking-cli.git
cd salon-booking-cli
2️⃣ Create the database
createdb salon

3️⃣ Restore database 
psql -d salon -f salon.sql

4️⃣ Run the script
./salon.sh
🧪 Example Flow
1) cut
2) trim
3) color
4) perm
5) style

What is your phone number?
The system will:

Check if the customer exists

Create a new customer if necessary

Ask for appointment time

Insert the appointment into the database

📚 What This Project Demonstrates
Interaction between Bash scripts and PostgreSQL

Handling user input in CLI environments

Relational database modeling

Managing sequences and identity reset

Structured procedural programming

Error handling and validation logic

🎯 Learning Purpose
This project was developed as part of backend/database practice and demonstrates how command-line applications can integrate with relational databases using SQL queries executed from shell scripts.

🧠 Future Improvements
Add input validation

Implement better error handling

Convert into REST API

Build web interface

Add authentication system

📄 License
This project is for educational purposes.
