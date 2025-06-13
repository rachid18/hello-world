# CRM Project

This repository contains a minimal Customer Relationship Management (CRM) system built with Django. It provides the base configuration for managing contacts and tracking sales activities.

## Development setup

Use a virtual environment to isolate dependencies:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Once the dependencies are installed, set up the database and start the server:

```bash
python manage.py migrate
python manage.py runserver
```

## Project architecture

The project follows a modular structure with separate Django apps:

- **crm_project** – root configuration and URL routing.
- **accounts** – user authentication and administration.
- **customers** – stores customer contact information.
- **sales** – manages leads and opportunities.

Each app encapsulates its own models, views and templates to keep the CRM easy to extend.
