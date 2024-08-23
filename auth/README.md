# Authentication
This directory contains the functionality related to authentication and user management in the MusicHUB application.

## Structure
```bash
auth/
├── auth.py # Authentication routes and views
├── forms.py # Authentication-related forms
├── models.py # User models
├── README.md # This README file
└── templates/ # Authentication templates (HTML files)
       └── login.html # Login page
       └── register.html # Registration page
       └── profile.html # User profile page
       └── login_register.html # Combined login and registration page
```

## Files

- **auth.py**: Contains the routes and views for managing authentication.
- **forms.py**: Contains the forms used for authentication-related operations.
- **models.py**: Contains the models for user authentication and management.
- **templates/**: Contains the HTML templates for authentication-related pages.

## Usage

To use the authentication functionality, import the necessary modules and include the routes in your Flask application.

```python
from auth.auth import auth
app.register_blueprint(auth)
```

Forms
The following forms are defined in [`forms.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fauth%2Fforms.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "auth/forms.py"):

- **LoginForm**: Form for user login.
- **RegisterForm**: Form for user registration.
- **ProfileForm**: Form for updating user profile.

Models
The following models are defined in [`models.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fauth%2Fmodels.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "auth/models.py"):

- **User**: Model representing a user.

## Routes

The following routes are defined in [`auth.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fauth%2Fauth.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "auth/auth.py"):

- **/register**: Route for user registration.
- **/login**: Route for user login.
- **/login_register**: Route for combined login and registration page.
- **/landing-page**: Route for the landing page (requires login).
- **/logout**: Route for user logout.
- **/profile**: Route for user profile (requires login).