# Root
This directory contains the root-level functionality for the MusicHUB application.

## Structure
```bash
root/
├── forms.py # Root-related forms
├── README.md # This README file
├── root.py # Root routes and views
└── templates/ # Root templates (HTML files)
    ├── root.html # Root details page
    ├── roots.html # Root list page
    ├── create_root.html # Root creation page
    └── update_root.html # Root update page
```

## Files

- **forms.py**: Contains the forms used for root-related operations.
- **root.py**: Contains the routes and views for managing root-level functionality.
- **templates/**: Contains the HTML templates for root-related pages.

## Usage

To use the root functionality, import the necessary modules and include the routes in your Flask application.

```python
from root.root import root_blueprint
app.register_blueprint(root_blueprint)
```

Forms
The following forms are defined in forms.py:

- **RootForm**: Form for creating and updating root entries.
- **RootSearchForm**: Form for searching root entries.
- **RootFetchForm**: Form for fetching root details.
- **RootSearchSQLForm**: Form for searching root entries using SQL.