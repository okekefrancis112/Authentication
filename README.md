# Authentication

A Django authentication system with email verification, featuring user registration, login, and email-based account activation.

## Overview

A full-featured authentication flow built with Django, including:

- User signup with email confirmation
- Secure signin/signout
- Email-based account activation with token verification
- Custom authentication backend

## Features

- **Email Verification** — Account activation via email link
- **Token-based Activation** — Secure token generation for email confirmation
- **Custom Auth Backend** — Custom authentication logic
- **HTML Templates** — Signup, signin, activation success/failure pages

## Tech Stack

- **Python** 3.x
- **Django** — Web framework
- **Pipenv** — Dependency management
- **SQLite** — Database

## Getting Started

### Prerequisites

- Python 3.x
- Pipenv

### Installation

```bash
git clone https://github.com/okekefrancis112/Authentication.git
cd Authentication
pipenv install
pipenv shell
cd auth
python manage.py migrate
python manage.py runserver
```

## Project Structure

```
├── auth/
│   ├── auth/
│   │   ├── settings.py          # Django settings
│   │   └── urls.py              # Root URL config
│   ├── authentication/
│   │   ├── models.py            # User models
│   │   ├── views.py             # Auth views
│   │   ├── tokens.py            # Token generation
│   │   ├── urls.py              # Auth URLs
│   │   └── templates/           # HTML templates
│   └── manage.py
├── Pipfile
└── Pipfile.lock
```

## License

MIT
