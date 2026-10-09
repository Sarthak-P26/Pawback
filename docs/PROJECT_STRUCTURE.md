# Project structure

This repository was reorganized into a cleaner, easier-to-navigate layout while keeping the live app files in place.

## Main folders

- `archive/duplicate-files/` – duplicate or generated versioned files that were cluttering the root. These are kept for reference only.
- `docs/` – project documentation and structural notes.
- `frontend/` – built frontend assets for the PawHaven app.
- `logs/` – local runtime logs from the Vite frontend dev server.

## Active app files

The following files remain at the project root because they are the active Django app entry points and templates used by the app:

- `manage.py`
- `settings.py`
- `urls.py`
- `views.py`
- `admin.py`
- `apps.py`
- `forms.py`
- `staff_tags.py`
- `pet_extras.py`
- `base.html`
- `landing.html`
- `login.html`
- `register.html`
- and the remaining top-level HTML templates and media assets

## Why this structure helps

- The root directory is no longer filled with duplicate file names like `login (3).html` and `views (9).py`.
- Generated logs are kept separate from the app source.
- The repo now clearly distinguishes active files from archived duplicates.
- Future work can safely add new domains like `apps/`, `templates/`, `static/`, and `migrations/` without mixing them into the root.
