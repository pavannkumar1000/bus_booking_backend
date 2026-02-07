🚌 Travels Bus Booking Backend

A Django REST Framework backend for a bus booking system.
Manage buses, seats, users, and bookings with token-based authentication and an admin panel.

⚙️ Features

✅ User registration and login (Token Authentication)

✅ List all buses

✅ Retrieve bus details

✅ Seat booking with availability check

✅ View user bookings

✅ Auto-create seats when a bus is added

✅ Admin panel for managing buses, seats, and bookings

📌 Dependencies

Python >= 3.10

Django >= 5.2

Django REST Framework

djangorestframework-authtoken

django-cors-headers

SQLite (default database)

All dependencies are included in requirements.txt.

💻 Setup & Run Locally
1. Clone the repository
git clone https://github.com/pavannkumar1000/bus_booking_backend.git
cd travels

2. Create & activate virtual environment
python -m venv venv

# Windows
venv\Scripts\activate

# Linux / macOS
source venv/bin/activate

3. Install dependencies
pip install -r requirements.txt

4. Run migrations
python manage.py makemigrations
python manage.py migrate

5. Load dummy bus data
python manage.py loaddata bookings/fixtures/buses.json

6. Create superuser (for admin panel)
python manage.py createsuperuser

7. Run development server
python manage.py runserver


Access the API at: http://127.0.0.1:8000/

Admin panel: http://127.0.0.1:8000/admin