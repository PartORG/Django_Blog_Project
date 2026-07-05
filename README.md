# Django_Blog_Project

A simple yet powerful blog website built with Django, designed to help developers quickly set up and manage their blogs.

[![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)] [![License](https://img.shields.io/github/license/PartORG/Django_Blog_Project.svg)] [![Django](https://img.shields.io/badge/django-3.2-green.svg)] [![Testing](https://img.shields.io/badge/tests-not%20available-red.svg)]

## Introduction

Welcome to Django_Blog_Project! This project is a straightforward example of a blog website built using the popular Python web framework, Django. It provides a solid foundation for developers looking to quickly set up and manage their blogs without having to reinvent the wheel.

The primary workflow involves creating posts, comments, and managing user interactions. The main advantages of this project include its simplicity, flexibility, and ease of customization.

## Features

### Post Management
- **Create Posts**: Easily add new blog posts with a simple form.
- **Edit Posts**: Update existing posts directly from the admin panel.
- **Delete Posts**: Remove unwanted posts without any hassle.

### Comment System
- **Add Comments**: Allow readers to leave comments on posts.
- **Moderate Comments**: Approve or reject comments manually.

### User Authentication
- **Login/Logout**: Secure user authentication with Django's built-in system.
- **User Profiles**: Optionally create and manage user profiles.

## How It Works

Django_Blog_Project is a typical Django project structured as follows:

1. **my_site/**: The main project directory containing settings, URLs, and WSGI configuration.
2. **blog/**: The app directory where the blog-related logic resides.

The core components of the project include:
- **models.py**: Defines the data models for posts and comments.
- **views.py**: Handles the business logic and renders templates.
- **urls.py**: Maps URLs to views.
- **templates/blog/**: Contains HTML templates for different pages.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| Django     | The web framework used to build the blog. |
| Python     | The programming language used. |
| SQLite     | The database used for storing blog data. |

## Requirements

To run this project, you need:
- Python 3.8 or higher
- Django 3.2 or higher

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/PartORG/Django_Blog_Project.git
   ```

2. Navigate to the project directory:
   ```sh
   cd Django_Blog_Project/my_site
   ```

3. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

4. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

5. Run migrations:
   ```sh
   python manage.py migrate
   ```

6. Create a superuser (for admin access):
   ```sh
   python manage.py createsuperuser
   ```

7. Start the development server:
   ```sh
   python manage.py runserver
   ```

## Configuration

The project uses environment variables for configuration. You can set these in your `.env` file or directly in your operating system's environment.

| Variable       | Description                  |
|----------------|------------------------------|
| `SECRET_KEY`     | The secret key for Django.     |
| `DEBUG`          | Enable/Disable debug mode.   |

## Quick Start

1. Clone the repository and navigate to the project directory.
2. Set up a virtual environment and install dependencies.
3. Run migrations and create a superuser.
4. Start the development server.

```sh
git clone https://github.com/PartORG/Django_Blog_Project.git
cd Django_Blog_Project/my_site
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

## Usage

To access the blog, open your web browser and navigate to `http://127.0.0.1:8000/`.

- **Admin Panel**: Accessed at `http://127.0.0.1:8000/admin/` using the superuser credentials.
- **Blog Posts**: View all posts at `http://127.0.0.1:8000/blog/`.
- **Post Detail**: View a specific post by visiting its URL.

## Project Structure

```
my_site/
├── blog/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── migrations/
│   │   ├── 0001_initial.py
│   │   ├── 0002_remove_post_image_name_post_image.py
│   │   ├── 0003_comment.py
│   │   ├── 0004_rename_name_comment_user_name.py
│   │   └── __init__.py
│   ├── models.py
│   ├── static/
│   │   ├── blog/
│   │   │   ├── all-posts.css
│   │   │   ├── images/
│   │   │   ├── index.css
│   │   │   ├── post-detail.css
│   │   │   └── post.css
│   │   └── app.css
│   ├── templates/
│   │   ├── blog/
│   │   │   ├── all-posts.html
│   │   │   ├── includes/
│   │   │   │   └── post.html
│   │   │   ├── index.html
│   │   │   ├── post-detail.html
│   │   │   └── stored-posts.html
│   │   └── base.html
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── db.sqlite3
├── manage.py
└── my_site/
    ├── __init__.py
    ├── settings.py
    ├── urls.py
    └── wsgi.py
```

## Development

The project follows a standard Django development workflow. You can add new features, modify existing ones, and run tests using the following commands:

- **Run Tests**: `python manage.py test`
- **Create Migrations**: `python manage.py makemigrations blog`
- **Migrate Database**: `python manage.py migrate`

## Limitations

- The project does not include advanced features like user authentication or a commenting system.
- Testing is not implemented.

## License

This project is licensed under the [MIT License](LICENSE).