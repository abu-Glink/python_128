
1. Environment Setup and Project Creation:
    Create and activate a virtual environment.
   
    Code
    python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   
    install django.
    Code
    pip install django
    Start a new Django project.
   
    Code
    django-admin startproject project_name .  # The dot creates the project in the current directory

3. Database Migrations:
    Create database migrations for built-in apps:

    Code
    python manage.py migrate

4. Running the Development Server:
    Start the Django development server.
   
    Code
    python manage.py runserver

5. Creating a Django App (Optional, but common):
    Create a new Django app within your project:
   
    Code
    python manage.py startapp app_name
    Add the new app to INSTALLED_APPS in project_name/settings.py: 
    Python
    # project_name/settings.py
    INSTALLED_APPS = [
        # ... other built-in apps
        'app_name',
    ]

6. Database Migrations for Custom Apps:
    Create migrations for your new app's models:
    Code
    python manage.py makemigrations app_name
    Apply the migrations to the database.
   
    Code
    python manage.py migrate
7. Creating a Superuser (Optional):
    Create an administrator user for the Django admin interface:
   
    Code
    python manage.py createsuperuser

