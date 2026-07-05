# Django Blog Project

A simple blog website built with Django, designed for learning and demonstration purposes.

## Requirements

- Python 3.10
- Django 4.0

## Installation

To set up the project locally:

1. Clone the repository:
   ```sh
   git clone https://github.com/PartORG/Django_Blog_Project.git
   ```

2. Navigate to the project directory:
   ```sh
   cd Django_Blog_Project/my_site
   ```

3. Install dependencies using pip:
   ```sh
   pip install -r requirements.txt
   ```

4. Run migrations:
   ```sh
   python manage.py migrate
   ```

5. Create a superuser (optional):
   ```sh
   python manage.py createsuperuser
   ```

6. Start the development server:
   ```sh
   python manage.py runserver
   ```

## Usage

To run the project, execute:

```sh
python manage.py runserver
```

This will start a local development server at `http://127.0.0.1:8000/`. You can access your blog by navigating to this URL in your web browser.

For more detailed instructions on how to use the project, refer to the [Django documentation](https://docs.djangoproject.com/en/stable/).