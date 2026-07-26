# Learning Log

>A full-stack web application built with Python and Django. This project is a hands-on learning log application created while following along with Eric Matthes's *"Python Crash Course (3rd Edition)".*


## Project Overview

>I am building this project as a fun way to brush up on my core Python skills and gain a practical understanding of the *Django web framework*, model-view-template (MVT) architecture, web security (CSRF, authentication), and cloud deployment.

>*"Learning Log"* allows users to log topics they are interested in and make timestamped entries as they learn new material.


## Tech Stack & Development Environment

> - *Language:* Python 3.12.11
> - *Framework:* Django 6.0.7
> - *Database:* SQLite (Development)
> - *Environment:* lightning.ai Cloud Studio / Linux (Zsh)
> - *Version Control:* Git & GitHub


## Project Roadmap & Implementation Log

### Phase 1: Environment & Project Setup (Up until initial commit)

> - Started Django project structure:
  ```bash
  django-admin startproject ll_project .
  ```
> - Configured development server settings (`ALLOWED_HOSTS` and `CSRF_TRUSTED_ORIGINS` for cloud proxy domain hosting).
> - Created the main application `learning_logs`:
  ```bash
  python manage.py startapp learning_logs
  ```
> - Defined the `Topic` model in `learning_logs/models.py`:
> - Created and applied database migrations:
  ```bash
  python manage.py makemigrations learning_logs
  python manage.py migrate
  ```
> - Registered `Topic` with the Django Admin site in `admin.py`.
> - Created a superuser account and populated initial test topics via Django Admin.
> - Initialized project repository on GitHub.

***To be continued...***

## How to Run Locally / In Development

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Sadi-Mahmud-Shurid/learning_log.git
   cd learning_log
   ```

2. **Install dependencies:**
   ```bash
   pip install django
   ```

3. **Apply database migrations:**
   ```bash
   python manage.py migrate
   ```

4. **Run the development server:**
   ```bash
   python manage.py runserver
   ```

5. **Access the application:**
    > - *Homepage:* `http://localhost:8000/` or your cloud proxy URL.
    > - *Admin Panel:* `http://localhost:8000/admin/`