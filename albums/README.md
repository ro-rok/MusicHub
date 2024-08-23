# Albums
This directory contains the functionality related to albums in the MusicHUB application.

## Structure
```bash
albums/
├── albums.py # Album routes and views
├── forms.py # Album-related forms
├── README.md # This README file
└── templates/ # Album templates (HTML files)
       └── album_manage.html # Album management page
       └── album_list.html # Album list page
       └── album_details.html # Album details page
```

## Files

- **albums.py**: Contains the routes and views for managing albums.
- **forms.py**: Contains the forms used for album-related operations.
- **templates/**: Contains the HTML templates for album-related pages.

## Usage

To use the album functionality, import the necessary modules and include the routes in your Flask application.

```python
from albums.albums import albums
app.register_blueprint(albums)
```

Forms
The following forms are defined in [`forms.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Falbums%2Fforms.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "albums/forms.py"):

- **AlbumForm**: Form for creating and updating albums.
- **AlbumSearchForm**: Form for searching albums.
- **AlbumFetchForm**: Form for fetching album details.
- **AlbumSearchSQLForm**: Form for searching albums using SQL.

Routes
The following routes are defined in [`albums.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Falbums%2Falbums.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "albums/albums.py"):

- **/add**: Route for adding a new album.
- **/edit**: Route for editing an existing album.
- **/delete**: Route for deleting an album.
- **/list**: Route for listing all albums.
- **/search**: Route for searching albums.
- **/view**: Route for viewing album details.
- **/fetch**: Route for fetching album details.