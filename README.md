# Django School Management System

A comprehensive Django-based school management application for managing students, teachers, courses, and academic records.

## Features

- **Student Management**: Track student information, enrollment, and academic progress
- **Teacher Management**: Manage teacher profiles and assignments
- **Course Management**: Create and organize courses with schedules
- **Grades & Reports**: Record grades and generate academic reports
- **Attendance Tracking**: Monitor student attendance
- **Admin Dashboard**: User-friendly interface for school administrators

## Tech Stack

- **Backend**: Django 4.x
- **Database**: PostgreSQL / SQLite (configurable)
- **Frontend**: Django Templates + Bootstrap
- **API**: Django REST Framework (optional)

## Installation

### Prerequisites
- Python 3.8+
- pip
- virtualenv

### Setup

1. Clone the repository
```bash
git clone https://github.com/karita2005/django-school-management.git
cd django-school-management
```

2. Create and activate virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Configure environment variables
```bash
cp .env.example .env
```

5. Run migrations
```bash
python manage.py migrate
```

6. Create a superuser
```bash
python manage.py createsuperuser
```

7. Start the development server
```bash
python manage.py runserver
```

Visit `http://localhost:8000/admin` to access the admin panel.

## Project Structure

```
django-school-management/
├── manage.py
├── requirements.txt
├── .env.example
├── .gitignore
├── config/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
├── apps/
│   ├── students/
│   │   ├── models.py
│   │   ├── views.py
│   │   └── urls.py
│   ├── teachers/
│   ├── courses/
│   ├── grades/
│   └── attendance/
├── templates/
│   └── base.html
└── static/
    └── css/
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
