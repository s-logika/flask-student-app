# 🐍 Student Introduction Flask App

A beginner-friendly Flask web application that demonstrates routing, dynamic URL parameters, and simple logic — built for learning Flask fundamentals.

---

## 📁 Project Structure

```
├── app.py            # Main Flask application
├── requirements.txt  # Python dependencies
├── .gitignore        # Files which ignored from git
└── README.md         # Project documentation
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <your-repo-url>
cd <your-repo-folder>
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the App

```bash
python app.py
```

The app will start at: **http://127.0.0.1:5000**

---

## 🛣️ Available Routes

| Route                       | Method | Description                    | Example                             |
| --------------------------- | ------ | ------------------------------ | ----------------------------------- |
| `/`                         | GET    | Home page                      | http://127.0.0.1:5000/              |
| `/about`                    | GET    | About page                     | http://127.0.0.1:5000/about         |
| `/contact`                  | GET    | Contact page                   | http://127.0.0.1:5000/contact       |
| `/student/<name>`           | GET    | Greet a student by name        | http://127.0.0.1:5000/student/John  |
| `/square/<number>`          | GET    | Returns the square of a number | http://127.0.0.1:5000/square/5      |
| `/cube/<number>`            | GET    | Returns the cube of a number   | http://127.0.0.1:5000/cube/3        |
| `/greet/<name>/<age>`       | GET    | Greet with name and age        | http://127.0.0.1:5000/greet/John/20 |
| `/triangle/<size>/<symbol>` | GET    | Prints a triangle pattern      | http://127.0.0.1:5000/triangle/5/*  |

---

## 📌 Route Examples & Output

### Home Page

```
GET /
→ Welcome to Flask Class
```

### Student Greeting

```
GET /student/Alice
→ Hello Alice, Welcome to Flask
```

### Square of a Number

```
GET /square/6
→ Square is 36
```

### Cube of a Number

```
GET /cube/3
→ cube of 3 is 27
```

### Greet with Age

```
GET /greet/John/20
→ Hi John! You are 20 years old.
```

### Triangle Pattern

```
GET /triangle/5/*
→
*
**
***
****
*****
```

> You can use any symbol: `/triangle/4/#`, `/triangle/3/@`

---

## 🧰 Requirements

- Python 3.x
- Flask

Install with:

```bash
pip install flask
```

Or use the provided `requirements.txt`:

```bash
pip install -r requirements.txt
```

---

## 💡 Concepts Covered

- Creating a Flask app instance
- Static routes (`/`, `/about`, `/contact`)
- Dynamic string routes (`/student/<name>`)
- Dynamic integer routes (`/square/<int:number>`)
- Multiple URL parameters (`/greet/<name>/<int:age>`)
- Returning HTML in responses (`<pre>` tag for formatting)
- Running loops and building string responses

---

## 📝 License

This project is intended for educational purposes.
