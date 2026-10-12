# Watchlist_python

A Python desktop application for managing a personal movie watchlist. Built with PySide6, it includes user accounts, personal movie collections, a sample movie catalog and statistics.

## Features

- User login and registration.
- Storage of user data in JSON files.
- Manual addition, editing and removal of movies.
- Movie status changes between `Do obejrzenia` (To watch) and `Obejrzano` (Watched).
- Recording the date a movie was watched.
- Searching a user's movie collection.
- Sorting movies by title, year and rating.
- Adding movies from the sample catalog.
- Adding comments to movies in the sample catalog.
- Viewing a history of watched movies.
- Exporting a personal movie list to a TXT file.
- Charts showing ratings of watched movies, movies by genre, watched versus unwatched movies, and the three highest-rated movies.

## Tech Stack

- Python
- PySide6
- matplotlib
- JSON for data storage

## Getting Started

Requirements:

- Python 3
- PySide6
- matplotlib

From the repository root, create a virtual environment, install dependencies and start the application:

```bash
cd projekt
python -m venv .venv
source .venv/bin/activate
pip install PySide6 matplotlib
python main.py
```

On Windows, use this activation command instead:

```bat
.venv\Scripts\activate
```

## Data

The project includes the following sample files:

```text
projekt/data/sample_movies.json
projekt/data/users.json
projekt/moje_filmy_admin.txt
```

`sample_movies.json` stores the sample movie catalog. `users.json` stores user data and personal movie lists.

## Project Structure

```text
projekt/
├── data/               # User data and sample movies in JSON format
├── exceptions/         # Custom exceptions
├── gui/                # PySide6 application windows
├── managers/           # Movie and user management logic
├── models/             # Movie and User models
├── utils/              # File export and statistics
└── main.py             # Application entry point
```

## Notes

The repository does not include a `requirements.txt` file. In the current implementation, user passwords are stored as plain text in JSON. Treat the project as an educational demonstration; the authentication implementation requires changes before production use.
