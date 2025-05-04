Django Web Application with Authentication

This is a fully functional web application built using Django that includes user authentication features such as login, registration, logout, and password reset. The application also demonstrates role-based user permissions.

 🔧 Features
- ✅ User Registration
- ✅ Secure Login and Logout
- ✅ Password Hashing using Django’s built-in authentication system
- ✅ Password Reset via Email
- ✅ Role-based Access Control (Admin and Regular User)

🚀 Technologies Used
- Python 3.10+  
- Django 5.x  
- HTML5, CSS3  
- SQLite (default Django database)  
- Bootstrap (for styling, optional)

📁 Project Structure
Django-Web-Application-with-Authentication/
│
├── myproject/ # Django project directory
│ ├── settings.py # Project settings
│ ├── urls.py # URL routing
│ └── ...
├── users/ # Custom app for user authentication
│ ├── views.py # Login, Register, Password reset views
│ ├── forms.py # User registration/login forms
│ └── ...
├── templates/ # HTML templates
│ └── registration/ # Password reset email templates
├── db.sqlite3 # Default database
└── manage.py # Django management script

🧑‍💻 User Roles
- Admin: Has access to Django admin panel and full permissions.
- Regular User: Can register, log in, reset password, and access user-specific pages.

 📬 Password Reset
The password reset feature is integrated using Django’s default email backend. Configure your SMTP settings in settings.py:

EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
EMAIL_HOST = 'smtp.gmail.com'
EMAIL_PORT = 587
EMAIL_HOST_USER = 'your_email@example.com'
EMAIL_HOST_PASSWORD = 'your_password'
EMAIL_USE_TLS = True
Replace the above credentials with your email account details or use environment variables for better security.

🛠️ Setup Instructions
Clone the repository
git clone https://github.com/jyo-022/Task-1-Django-Web-Application-with-Authentication.git
cd Task-1-Django-Web-Application-with-Authentication


Create a virtual environment and activate it
python -m venv venv
venv\Scripts\activate   # On Windows

Install dependencies
pip install -r requirements.txt

Apply migrations
python manage.py migrate

Create a superuser (for admin access)
python manage.py createsuperuser

Run the server
python manage.py runserver


Access the site
Open http://127.0.0.1:8000 in your browser.
Admin panel: http://127.0.0.1:8000/admin



📄 License
This project is licensed under the MIT License.
Feel free to use and modify it as per your needs.

Made with ❤️ using Django.
