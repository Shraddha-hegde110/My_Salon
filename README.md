# 💇‍♀️ My Salon Appointment Scheduler

This is a command-line based appointment booking system for a salon, built as part of the [freeCodeCamp Relational Database Certification](https://www.freecodecamp.org/learn). It uses **Bash scripting** for logic and **PostgreSQL** as the backend database.

---

## 🧾 Features

- View list of available salon services.
- Enter customer details and schedule appointments.
- Automatically stores appointment data in PostgreSQL.
- Creates new customer entries if not already registered.

---

## 📂 Project Structure

```bash
My_Salon-main/
│
├── salon.sh      # Main Bash script for appointment logic
└── salon.sql     # SQL schema for database setup
```

---

## ⚙️ Prerequisites

- PostgreSQL installed and running
- Bash shell (Linux/macOS or Git Bash on Windows)
- `psql` command-line tool

---

## 🛠️ Setup Instructions

### 1. Create the database

Open terminal and run:

```bash
psql -U postgres -f salon.sql
```

This will create the required database and tables.

### 2. Run the script

```bash
./salon.sh
```

If it shows a permission error, make it executable first:

```bash
chmod +x salon.sh
./salon.sh
```

---

## 🧪 Example Usage

```
Welcome to My Salon, how can I help you?
1) Cut
2) Color
3) Wash
...
Please enter your phone number: 1234567890
I don't have a record for that phone number, what's your name? Shraddha
What time would you like your Cut, Shraddha? 3pm
I have put you down for a Cut at 3pm, Shraddha.
```

---

## 🧹 Troubleshooting

- Ensure PostgreSQL service is running.
- Check if the database name in `salon.sh` matches the one created.
- Use correct username when running `psql`.

---

## 📜 License

This project is for educational purposes and licensed under [MIT](LICENSE) if applicable.

---

## ✨ Credits

Built by Shraddha Hegde as part of freeCodeCamp’s Relational Database certification.
