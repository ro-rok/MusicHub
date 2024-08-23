# Tracks
This directory contains the functionality related to tracks in the MusicHUB application.

## Structure
```bash
tracks/
├── tracks.py # Track routes and views
├── forms.py # Track-related forms
├── README.md # This README file
└── templates/ # Track templates (HTML files)
       └── track.html # Track details page
       └── tracks.html # Track list page
       └── create_track.html # Track creation page
       └── update_track.html # Track update page
```

## Files

- **tracks.py**: Contains the routes and views for managing tracks.
- **forms.py**: Contains the forms used for track-related operations.
- **templates/**: Contains the HTML templates for track-related pages.

## Usage

To use the track functionality, import the necessary modules and include the routes in your Flask application.

```python
from tracks.tracks import tracks
app.register_blueprint(tracks)
```

Forms
The following forms are defined in [`forms.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Ftracks%2Fforms.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "tracks/forms.py"):

- **TrackForm**: Form for creating and updating tracks.
- **TrackSearchForm**: Form for searching tracks.
- **TrackFetchForm**: Form for fetching track details.
- **TrackSQLSearchForm**: Form for searching tracks using SQL.