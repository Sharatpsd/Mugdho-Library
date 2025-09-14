# 📚 Mugdho Library Management System

**Author / Developer:** Sharat Acharjee Mugdho  
**Portfolio:** [https://mugdho-portfolio.netlify.app](https://mugdho-portfolio.netlify.app)  
**GitHub:** [https://github.com/Sharatpsd](https://github.com/Sharatpsd)  

This is a professional library management system built for academic and portfolio purposes. It demonstrates **Django, Django REST Framework, and Python backend skills**, along with **user authentication, CRUD operations, and fine management**.
## 📖 Screenshots

### Figure 1: Books List Grid View
![Books List Grid View](https://drive.google.com/uc?export=view&id=1rg5FMsyxXoTz_PI2hevhqO8eeiR9tRb5)

### Figure 2: Books List Grouped View
![Books List Grouped View](https://drive.google.com/uc?export=view&id=10pbwq5bLl4ZB3OIAnlWGuWDVakxfF5IK)

### Figure 3: Books List with Diverse Authors
![Books List with Diverse Authors](https://drive.google.com/uc?export=view&id=1p1piQVbaJ-ZWjqfM3Kp-EH-yfevZGM6s)

### Figure 4: Admin Dashboard - All Issues
![Admin Dashboard - All Issues](https://drive.google.com/uc?export=view&id=14HZlt2qmiTLuHPbgBZ2LzR5m77BYUocq)

---

## 🔧 Technologies Used
- **Frontend:** HTML5, CSS3, Tailwind CSS, Vanilla JavaScript  
- **Backend:** Python, Django, Django REST Framework (DRF)  
- **Database:** SQLite (default, can switch to PostgreSQL)  
- **Payment Integration:** RazorPay  
- **Deployment:** Can be deployed on Render, Railway, Heroku, or any cloud hosting  

---

## 🚀 Features

### General
1. Browse all books
2. Search and filter by author, book name, or category
3. Sort books/authors alphabetically

### Student Features
1. Signup/Login  
2. Request and view book issues  
3. Check fines and overdue books  
4. Pay fines online through RazorPay  
5. View remaining days to return books or overdue duration  

### Admin Features
1. Login to admin dashboard  
2. Manage books and authors (add, delete, search, filter)  
3. Manage student accounts and their issues/fines  
4. Accept or reject book issue requests  
5. Calculate fines automatically or manually  
6. Toggle fine paid status  

### Additional Features
- Student signup validates unique student ID  
- Book availability shows status (`issued`, `issue requested`, or `request issue`)  

---

## 📂 Project Structure (Summary)
django-library-management/
│
├─ core/ # Project settings
├─ library/ # Library app (models, views)
├─ student/ # Student app (authentication)
├─ templates/ # HTML templates
├─ static/ # CSS/JS files
├─ manage.py
└─ README.md

yaml
Copy code

---


---

## ⚙️ How to Run Locally
1. Clone the repository:  
```bash
git clone https://github.com/Sharatpsd/Mugdho-Library.git
Create virtual environment & activate:

bash
Copy code
python -m venv .venv
.\.venv\Scripts\activate   # Windows
source .venv/bin/activate  # Mac/Linux
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Create .env file and add:

ini
Copy code
SECRET_KEY=<your_secret_key>
RAZORPAY_KEY_ID=<your_razorpay_id>
RAZORPAY_KEY_SECRET=<your_razorpay_secret>
Run migrations:

bash
Copy code
python manage.py migrate
Create superuser for admin:

bash
Copy code
python manage.py createsuperuser
Run server:

bash
Copy code
python manage.py runserver
Visit http://127.0.0.1:8000/

💡 Important Logic
Student ID: Django User username

Sign Up: Creates User + Student instance

Calculate Fine: Checks issued books, return status, overdue, updates Fine model

Payment: RazorPay integration handles online payment and updates status

Made with ❤️ by Sharat Acharjee Mugdho
Portfolio: https://mugdho-portfolio.netlify.app | GitHub: https://github.com/Sharatpsd
