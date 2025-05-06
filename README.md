# FINAL_project-ce-3
README - Django & Flask API Hotel Booking Project
==================================================

Project Title:
--------------
Hotel Booking System with Django Frontend and Flask Backend API

Description:
------------
This project is a hotel booking platform combining the power of Django for the frontend and admin panel, with Flask providing a lightweight RESTful API backend for handling certain dynamic operations like room availability, bookings, and mock payments.

Features:
---------
- User registration and login (Django Authentication)
- Admin control panel to add/update/delete Hotels and Rooms (Django Admin)
- Room listing and booking interface
- RESTful APIs for:
    - Fetching available rooms
    - Creating bookings
    - Payment simulation
- Secret and settings stored securely using `.env` files

Technologies Used:
------------------
- Django
- Flask
- SQLite (or other configured DB)
- HTML/CSS (for frontend templates)
- REST API (Flask + Flask-Restful or Flask API)
- Postman for API testing

Project Structure:
------------------
/final-evaluation/
├── django_project/
│   ├── final/                # Django project root
│   ├── home/                 # Django app for hotel booking
│   ├── templates/            # HTML templates
│   ├── static/               # CSS/JS files
├── flask_api/
│   ├── app.py                # Flask API routes
│   ├── api_models.py         # Models for API
│   ├── api_routes.py         # RESTful endpoints
├── requirements.txt
├── README.txt
├── .env                      # For secrets (ignored in git)

Setup Instructions:
-------------------
1. Clone the repository:
   git clone https://github.com/divyanshusharma011/final-evaluation.git

2. Navigate to the Django project:
   cd final-evaluation/django_project

3. Set up virtual environment and install Django dependencies:
   python -m venv venv
   source venv/bin/activate (Linux/Mac) or venv\Scripts\activate (Windows)
   pip install -r requirements.txt

4. Apply migrations and start the Django server:
   python manage.py makemigrations
   python manage.py migrate
   python manage.py runserver

5. Navigate to Flask API directory and run Flask backend:
   cd ../flask_api
   source ../venv/bin/activate
   python app.py

6. Access:
   - Django site: http://127.0.0.1:8000
   - Flask API: http://127.0.0.1:5000/api/

Environment Variables:
----------------------
Store sensitive data in a `.env` file like:

    SECRET_KEY=your_django_secret
    DATABASE_URL=sqlite:///db.sqlite3
    API_KEY=your_api_key_here

Note: `.env` is ignored in git. DO NOT expose secrets.

Contributing:
-------------
Pull requests are welcome. Please open an issue first to discuss proposed changes.

License:
--------
This project is open-source and available under the MIT License.
#
