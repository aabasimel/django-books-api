# Django Books API

A simple RESTful API built with **Django** and **Django REST Framework** to manage a collection of books.  
This project demonstrates creating models, serializers, and class-based API views in Django.

---

## Features

- List all books (`GET /api/books/`)  
- Create a new book (`POST /api/books/`)  
- Uses **ModelSerializer** for automatic JSON serialization  
- Follows Django REST Framework best practices

---

## Project Structure

my_project1/
├── my_app/ # Django app containing models, views, serializers
│ ├── migrations/
│ ├── models.py # Book model
│ ├── serializers.py # BookSerializer
│ ├── views.py # API views
│ └── urls.py # App-level URL routes
├── my_project1/ # Project settings
│ ├── settings.py
│ ├── urls.py # Project-level URL routes
│ └── wsgi.py
├── manage.py # Django management script
└── README.md


---

## Getting Started

### Prerequisites

- Python 3.12+  
- Django 5.2+  
- Django REST Framework

### Installation

1. Clone the repository:

```bash
git clone https://github.com/aabasimel/django-books-api.git
cd django-books-api
```
2. Create a virtual environment and activate it:
```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```
3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Apply database migrations:
```bash
python manage.py makemigrations
python manage.py migrate
```
5. Run the development server:
```bash
python manage.py runserver
```
6.Open your browser or Postman and visit:

http://127.0.0.1:8000/api/books/
