# Scholarship Management System 🎓

A web-based Scholarship Management System designed to simplify and automate the scholarship application and management process for students and administrators.

---

# 📌 Overview

The Scholarship Management System helps educational institutions manage scholarship applications digitally. Students can apply for scholarships online, while administrators can review, approve, or reject applications through an admin dashboard.

This project reduces paperwork, improves efficiency, and provides a user-friendly platform for scholarship management.

---

# ✨ Features

## 👨‍🎓 Student Module
- Student Registration
- Student Login Authentication
- Apply for Scholarships
- Upload Required Documents
- View Application Status
- Manage Profile

## 👨‍💼 Admin Module
- Admin Login
- View All Applications
- Approve or Reject Applications
- Manage Scholarship Details
- Database Management
- Dashboard Interface

## 🔒 Security Features
- Secure Login System
- Data Validation
- Protected User Information

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Backend Development |
| Flask | Web Framework |
| HTML | Frontend Structure |
| CSS | Styling |
| Bootstrap | Responsive UI |
| SQLite / MySQL | Database |
| JavaScript | Frontend Interactivity |

---

# 📦 Required Libraries

Install all required libraries using:

```bash
pip install flask flask_sqlalchemy flask_login werkzeug
```

Or install using requirements.txt:

```bash
pip install -r requirements.txt
```

---

# 📄 requirements.txt

Create a file named:

```bash
requirements.txt
```

Add this inside:

```txt
Flask
Flask-SQLAlchemy
Flask-Login
Werkzeug
```

---

# 📂 Project Structure

```bash
Scholarship-Management-System/
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── templates/
│   ├── index.html
│   ├── login.html
│   ├── register.html
│   ├── dashboard.html
│   └── admin.html
│
├── database/
│
├── app.py
├── requirements.txt
├── README.md
└── scholarship.db
```

---

# 🚀 Installation & Setup

## Step 1 — Clone Repository

```bash
git clone https://github.com/your-username/scholarship-management-system.git
```

---

## Step 2 — Navigate to Project Folder

```bash
cd scholarship-management-system
```

---

## Step 3 — Create Virtual Environment (Optional)

```bash
python -m venv venv
```

### Activate Virtual Environment

#### Windows
```bash
venv\Scripts\activate
```

#### Mac/Linux
```bash
source venv/bin/activate
```

---

## Step 4 — Install Required Libraries

```bash
pip install -r requirements.txt
```

---

# 👨‍💼 Creating Admin User

There are multiple ways to create an admin account.

## Method 1 — Directly From Database

Open your database and change:

```txt
is_admin = True
```

for your account.

---

## Method 2 — Hardcoded Admin Login

Inside `app.py`:

```python
ADMIN_USERNAME = "admin"
ADMIN_PASSWORD = "admin123"
```

Example:

```python
@app.route('/admin-login', methods=['GET', 'POST'])
def admin_login():
    if request.method == 'POST':
        username = request.form['username']
        password = request.form['password']

        if username == "admin" and password == "admin123":
            return redirect('/admin-dashboard')

    return render_template('admin_login.html')
```

---

# 🔑 Default Admin Credentials

```txt
Username: admin
Password: admin123
```

---

# ▶️ Running the Project

Run the Flask application:

```bash
python app.py
```

Open browser and visit:

```bash
http://127.0.0.1:5000
```

---

# 📸 Screenshots

## Home Page
- User-friendly landing page

## Login Page
- Secure student/admin login system

## Dashboard
- Scholarship management dashboard

## Admin Panel
- Application approval/rejection interface

---

# 🎯 Objectives of the Project

- Digitize scholarship application process
- Reduce paperwork
- Improve transparency
- Save administrative time
- Provide easy access for students

---

# 💡 Future Enhancements

- Email Notifications
- AI-based Eligibility Prediction
- Online Document Verification
- Cloud Database Integration
- Mobile Application Support
- Payment Gateway Integration

---

# 📚 Learning Outcomes

Through this project, the following concepts were learned:

- Full Stack Web Development
- Database Connectivity
- Flask Framework
- User Authentication
- CRUD Operations
- Project Structuring
- Frontend & Backend Integration

---

# 🧠 Use Cases

- Colleges
- Universities
- Scholarship Portals
- Educational Institutions

---

# ⚙️ Requirements

```txt
Python 3.x
Flask
SQLite/MySQL
VS Code / PyCharm
```

---

# 🧪 Useful Commands

## Install Flask

```bash
pip install flask
```

## Check Installed Libraries

```bash
pip list
```

## Freeze Installed Libraries

```bash
pip freeze > requirements.txt
```

---

# 👨‍💻 Author

## Akash

Engineering Student passionate about:
- Python Development
- AI/ML
- Embedded Systems
- Robotics
- Automation Projects

---

# ⭐ GitHub Tips

If you like this project:

⭐ Star the repository  
🍴 Fork the project  
📢 Share with others

---

# 📄 License

This project is created for educational purposes only.

---

# ✅ Project Status

Completed Successfully ✔️
