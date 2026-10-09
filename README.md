# PawBack Project

A pet adoption and shelter management portal with a Django backend and a frontend build.

## Project structure

```text
project-root/
├── backend/                    # backend workspace / virtualenv area
├── docs/
│   └── PROJECT_STRUCTURE.md   # structure notes
├── frontend/
│   ├── dist/                   # built frontend bundle
│   └── node_modules/           # frontend dependencies
├── legacy/
│   ├── duplicates/             # one-off or duplicate legacy files
│   ├── migrations/             # old migration files kept out of the root
│   └── misc/                   # extra historical files
├── logs/                       # local runtime logs
├── static/
│   └── images/                 # static images and media assets
├── templates/                  # HTML templates
├── admin.py
├── apps.py
├── asgi.py
├── forms.py
├── manage.py
├── pet_extras.py
├── README.md
├── requirements.txt
├── settings.py
├── staff_tags.py
├── urls.py
├── views.py
└── ...project config files
```

## Getting started

1. Create and activate a Python virtual environment.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Django app:
   ```bash
   python manage.py runserver
   ```
4. Serve the frontend build locally if needed from the `frontend/` directory.

## Notes

- Template files were consolidated into `templates/`.
- Static images and media were consolidated into `static/images/`.
- Legacy and duplicate files were moved into `legacy/` to keep the root clean.
- Runtime logs are stored under `logs/` instead of cluttering the app folders.
- For more details, see [docs/PROJECT_STRUCTURE.md](docs/PROJECT_STRUCTURE.md).
