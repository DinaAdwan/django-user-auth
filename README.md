# Django User Management

User authentication flows built with Django's built-in auth system, during the Gaza Sky Geeks backend programme.

## Features
- Registration with a custom form that adds an email field, and automatic login after sign-up
- Login and logout
- Password change
- Password reset by email (emails are printed to the console in development)
- Dashboard page for logged-in users

## Tech
Python · Django 4.1 · `django.contrib.auth` · SQLite

## Run locally
```bash
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```
Then open `/register/`.

The secret key is read from the `DJANGO_SECRET_KEY` environment variable; a development fallback is used if it isn't set.
