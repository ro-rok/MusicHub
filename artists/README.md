# Artists
This directory contains the functionality related to artists in the MusicHUB application.

## Structure
```bash
artists/
├── artists.py # Artist routes and views
├── forms.py # Artist-related forms
├── README.md # This README file
└── templates/ # Artist templates (HTML files)
       └── artist.html # Artist details page
       └── artists.html # Artist list page
       └── create_artist.html # Artist creation page
       └── update_artist.html # Artist update page
```

## Files

- **artists.py**: Contains the routes and views for managing artists.
- **forms.py**: Contains the forms used for artist-related operations.
- **templates/**: Contains the HTML templates for artist-related pages.

## Usage

To use the artist functionality, import the necessary modules and include the routes in your Flask application.

```python
from artists.artists import artists
app.register_blueprint(artists)
```

Forms
The following forms are defined in [`forms.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fartists%2Fforms.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "artists/forms.py"):

- **ArtistForm**: Form for creating and updating artists.
- **ArtistSearchForm**: Form for searching artists.
- **ArtistFetchForm**: Form for fetching artist details.
- **ArtistSQLSearchForm**: Form for searching artists using SQL.

Routes
The following routes are defined in [`artists.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fartists%2Fartists.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "artists/artists.py"):

- **/add**: Route for adding a new artist.
- **/edit**: Route for editing an existing artist.
- **/delete**: Route for deleting an artist.
- **/list**: Route for listing all artists.
- **/search**: Route for searching artists.
- **/view**: Route for viewing artist details.
- **/fetch**: Route for fetching artist details.