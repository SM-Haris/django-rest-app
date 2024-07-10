# Django REST Backend

## Description

This Django project serves as a comprehensive demonstration of Django REST Framework's capabilities. It implements robust features, including:

* **RESTful API Design**: Endpoints adhere to RESTful principles, ensuring a clean and consistent API structure.
* **Authentication**: Secure access is provided using a custom implementation built upon Simple JWT for user authentication.
* **Authorization**: Fine-grained control over user permissions is not directly implemented in this example, but the groundwork can be laid for future integration.
* **Custom User Model**: A CustomUser class extends the default Django user model with additional fields or logic tailored to your application's needs.
* **Exception Handling**: Custom middlewares effectively catch and handle unhandled exceptions, providing informative error messages for debugging and user experience.
* **Audit Logging and Error Logging**: Essential actions and errors are logged to files for auditing, troubleshooting, and security purposes. Logs are rotated on a 5-day basis to manage storage efficiently.
* **User CRUD APIs**: Comprehensive REST APIs are created for user creation, retrieval, update, and deletion (CRUD) operations.
* **Token Refresh and Verification**: Dedicated API endpoints handle token refresh and verification for maintaining user sessions securely.
* **User Signup and Login**: Streamlined APIs facilitate user registration and login, allowing users to interact with the application.
* **Custom Mixins**: Reusable mixins are designed to simplify queryset filtering operations within your API views.
* **Serializers:** Serializer classes map between Python objects (models) and JSON representations, ensuring data integrity and efficient data exchange.
* **Search and Filtering**: Powerful query parameters leverage Django and REST Framework filters, enabling users to search and filter data based on specific criteria.
* **Database Connection**: The project is configured to connect to a PostgreSQL database for data storage and persistence.

## Prerequisites

* Python 3.x (Recommended: Use a virtual environment)
* pip (Package installer for Python)
* PostgreSQL database server
* Installation

## Clone the repository:
 
```Bash
git clone https://github.com/SM-Haris/django-rest-app.git
```

## Create a virtual environment (recommended for isolation):

```Bash
python -m venv venv
source venv/bin/activate  # For Linux/macOS
venv\Scripts\activate.bat  # For Windows
```

## Install project dependencies:

```Bash
pip install -r requirements.txt
```

## Apply database migrations:

```Bash
python manage.py migrate
```

### (Optional) Create a PostgreSQL database and configure connection details in settings.py.

## Start the development server:

```Bash
python manage.py runserver
```
Access the API in your web browser, typically at http://127.0.0.1:8000/.