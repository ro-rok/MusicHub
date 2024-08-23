# SQL
This directory contains the SQL scripts used to create and manage the database schema for the MusicHUB application.

## Structure
```bash
sql/
├── 000_create_table_sample.sql # Create Sample table
├── 001_create_table_users.sql # Create Users table
├── 002_create_table_roles.sql # Create Roles table
├── 007_create_table_tracks.sql # Create Tracks table
├── 008_create_table_artists.sql # Create Artists table
├── 009_create_table_albums.sql # Create Albums table
├── 012_create_table_albumartists.sql # Create ArtistAlbums table
├── 013_create_table_trackfeatures.sql # Create TrackFeatures table
└── init_db.py # Initialize the database
```


## Usage

To initialize the database, run the `init_db.py` script:

```sh
python sql/init_db.py
```

This will execute all the SQL scripts in the correct order to set up the database schema.