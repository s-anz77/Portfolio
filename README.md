# Personal Portfolio Website

A personal portfolio website built with Django. It introduces the developer, presents selected projects, and provides contact links.

**Live site:** [portfolio-anzore.up.railway.app](https://portfolio-anzore.up.railway.app/)

## Features

- Single-page portfolio with About, Projects, and Contacts sections.
- Project cards link to the community platform, course website, and shop demos.
- Contact links for email and Telegram.
- Responsive layout implemented with HTML and CSS.

## Tech stack

- Python 3.15
- Django 6.1
- HTML, CSS, and JavaScript
- SQLite
- WhiteNoise and Gunicorn for deployment

## Prerequisites

- Python 3.15
- pip

## Local setup

From the repository root, create and activate a virtual environment:

```bash
python -m venv .venv
```

Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

macOS/Linux:

```bash
source .venv/bin/activate
```

Install dependencies, apply migrations, and run the site:

```bash
python -m pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Open <http://127.0.0.1:8000/>.

## Configuration

The project uses SQLite at `db.sqlite3`. The current Django settings define the secret key in `Portfolio_2/settings.py`; no `.env` file or environment variable configuration is provided by the project. The deployment `Procfile` starts the app with Gunicorn.

## Project structure

- `Portfolio_2/` — Django settings, URL configuration, and WSGI/ASGI entry points.
- `main/` — the portfolio page view and template.
- `static/` — styles, scripts, images, and fonts used by the page.
- `manage.py` — Django management commands.

