# 🏦 Bank Transaction Management System

A simple **Flask-based web application** for managing personal bank transactions. Supports full **CRUD** (Create, Read, Update, Delete) operations plus transaction search by amount range.

---

## ✨ Features

- **View Transactions** — Display all transactions in a clean table layout.
- **Add Transaction** — Add a new transaction with a date and amount.
- **Edit Transaction** — Update the date or amount of an existing transaction.
- **Delete Transaction** — Remove a transaction from the list.
- **Search Transactions** — Filter transactions within a minimum and maximum amount range.
- **Responsive UI** — Styled with Bootstrap 4 and a warm gradient theme.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python 3   | Backend logic |
| Flask      | Web framework |
| Jinja2     | Templating engine |
| HTML5 / CSS3 | Frontend structure & styling |
| Bootstrap 4 | UI components and responsiveness |

---

## 📁 Project Structure

```
obmnl-flask_assignment/
├── app.py                  # Flask application (routes & logic)
├── templates/
│   ├── transactions.html   # View all transactions (Read)
│   ├── form.html           # Add new transaction form (Create)
│   ├── edit.html           # Edit transaction form (Update)
│   └── search.html         # Search transactions by amount range
└── README.md               # Project documentation (this file)
```

---

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.7 or higher installed on your system

### Steps

1. **Clone or navigate to the project directory**
   ```bash
   cd obmnl-flask_assignment
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**
   - On **Windows**:
     ```bash
     venv\Scripts\activate
     ```
   - On **macOS / Linux**:
     ```bash
     source venv/bin/activate
     ```

4. **Install Flask**
   ```bash
   pip install flask
   ```

5. **Run the application**
   ```bash
   python app.py
   ```

6. **Open in browser**
   Navigate to [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## 🚀 Usage

| Action | How to |
|--------|--------|
| **View all transactions** | Go to the homepage (`/`) |
| **Add a transaction** | Click the "Add Transaction" button and fill in the date & amount |
| **Edit a transaction** | Click the "Edit" button next to a transaction and modify the fields |
| **Delete a transaction** | Click the "Delete" button next to a transaction |
| **Search transactions** | Navigate to `/search` (or any page you wire the search link to), enter min/max amount, and click "Search" |

> ⚠️ **Note:** Data is stored **in memory** (a Python list). All transactions will be lost when the server is restarted.

---

## 🌐 API Routes

| Method | Route | Description |
|--------|-------|-------------|
| GET | `/` | Display all transactions |
| GET | `/add` | Show the "Add Transaction" form |
| POST | `/add` | Submit a new transaction |
| GET | `/edit/<int:transaction_id>` | Show the edit form for a specific transaction |
| POST | `/edit/<int:transaction_id>` | Submit updates for a specific transaction |
| GET | `/delete/<int:transaction_id>` | Delete a specific transaction |
| GET/POST | `/search` | Search transactions by amount range |

---

## 🎨 Styling

- **Background Gradient:** `linear-gradient(to right, #f6d365, #fda085)` — a warm sunset palette.
- **Cards/Tables:** White background with rounded corners and soft shadows for a clean, modern look.
- **Responsive:** Built with Bootstrap 4, so the UI adapts to different screen sizes.

---

## 📄 License

This project is for educational/demonstration purposes. Feel free to use and modify it as needed.

