
# MusicHUB 🎵

MusicHUB is a comprehensive platform designed to enhance your music listening experience by integrating Spotify's API with a custom-built application. Whether you're managing playlists, exploring new tracks, or curating your favorite artists and albums, MusicHUB brings everything under one roof with a user-friendly interface.

## Features 🚀

- **User Authentication**: Secure and customizable authentication system using Flask-WTF, supporting registration, login, and profile management.
- **Spotify API Integration**: Seamless integration with Spotify's API to fetch and manage tracks, albums, and artists.
- **Role-Based Access Control**: Advanced user role management, allowing you to assign roles and permissions dynamically.
- **Dynamic Playlists**: Create, update, and manage your playlists with real-time updates.
- **Search & Explore**: Find and discover new music based on your preferences.
- **Customizable Profiles**: Personalize your user profile with various settings and options.
- **Responsive Design**: Mobile-friendly and responsive design for a seamless experience across devices.


## Technologies Used 🛠️

- **Backend**: Flask, SQLAlchemy
- **Frontend**: Jinja2, HTML, CSS, JavaScript
- **Database**: MySQL
- **API Integration**: Spotify API
- **User Authentication**: Flask-WTF, WTForms
- **Role Management**: Flask-Principal

## Installation 📦

1. **Clone the repository**:
   ```bash
   git clone https://github.com/username/MusicHUB.git
   cd MusicHUB
    ```

2. **Create a virtual environment:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install the dependencies:**
   ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables:**
   - Create a `.env` file in the root directory.
   - Add the following environment variables:
     ```bash
     FLASK_APP=app.py
     FLASK_ENV=development
     SECRET_KEY=your_secret_key
     SPOTIPY_CLIENT_ID=your_client_id
     SPOTIPY_CLIENT_SECRET=your_client_secret
     SPOTIPY_REDIRECT_URI=http://localhost:5000/callback
     ```
    - Replace `your_secret_key`, `your_client_id`, and `your_client_secret` with your own values.

5. **Run the application:**
    ```bash
    flask run
    ```
    Open `http://localhost:5000` in your browser to access the application.

## Directory Structure 📁

```bash
MusicHUB
├── __init__.py # Initialize the Flask application
├── .github/ 
│   └── workflows/ # GitHub Actions workflows
├── .gitignore
├── albums/ # Album-related functionality
│   ├── albums.py # Album routes and views
│   ├── forms.py # Album-related forms
│   └── templates/ # Album templates (HTML files)
├── artists/ # Artist-related functionality
│   ├── artists.py # Artist routes and views
│   ├── forms.py # Artist-related forms
│   └── templates/ # Artist templates (HTML files)
├── auth/ # Authentication and user management 
│   ├── auth.py # Authentication routes and views
│   ├── forms.py # Authentication forms
│   ├── models.py # User models
│   └── templates/ # Authentication templates (HTML files)
├── common/ # Common utilities and helper functions
│   └── utils.py # Utility functions
├── Dockerfile # Docker configuration file
├── main.py # Main application file
├── README.md # Project README
├── requirements.txt # Python dependencies
├── roles/ # Role-based access control
│   ├── forms.py # Role-related forms
│   ├── models.py # Role models
│   ├── permissions.py # Role permissions 
│   ├── roles.py # Role routes and views 
│   └── templates/ # Role templates (HTML files)
├── root/ # Root routes and views
│   ├── forms.py # Root forms
│   ├── root.py # Root routes and views
│   └── templates/ # Root templates (HTML files)
├── sql/ # SQL database schema and queries
│   ├── 001_create_table_users.sql 
│   ├── 002_create_table_roles.sql
│   └── ...
├── static/ # Static files (CSS, JS, images)
│   └── ...
├── templates/ # Base templates (HTML files)
│   └── ...
├── test/ # Test cases
│   └── ...
├── tracks/ # Track-related functionality
│   ├── forms.py # Track-related forms
│   ├── templates/ # Track templates (HTML files)
│   └── tracks.py # Track routes and views
├── utils/ # Utility functions
│   └── SQLLoader.py # SQL query loader

```

## Contributing 🤝

Contributions are welcome! Feel free to raise issues, create pull requests, or suggest improvements to the project.

## License 📝

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements 🙏

- [Spotify API](https://developer.spotify.com/documentation/web-api/)
- [Flask](https://flask.palletsprojects.com/)
- [SQLAlchemy](https://www.sqlalchemy.org/)
- [WTForms](https://wtforms.readthedocs.io/)
- [Flask-WTF](https://flask-wtf.readthedocs.io/)
- [Flask-Principal](https://pythonhosted.org/Flask-Principal/)
- [Jinja2](https://jinja.palletsprojects.com/)
- [Bootstrap](https://getbootstrap.com/)
- [Font Awesome](https://fontawesome.com/)


## Orginal Project Link 🌐

Here is the link to the original project with all the commits and branches:
[MusicHUB](https://github.com/ro-rok/rk868-is601-007/tree/main/Spotify_Project)

