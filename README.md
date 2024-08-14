# Django-Ticketing

A ticket system created in the Django framework that allows users to create, update, and delete tickets for their IT department, which can reply to and change the tickets.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- User registration and login
- Ticket creation, editing, and deletion
- Admin interface for viewing and responding to tickets
- Email notifications for updates on ticket status

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/NahimMK/Django-Ticketing.git
   cd Django-Ticketing
   ```

2. **Create and activate a virtual environment** (optional but recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install the dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations to set up the database**:
   ```bash
   python manage.py migrate
   ```

5. **Create a superuser account** (for accessing the admin interface):
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the development server**:
   ```bash
   python manage.py runserver
   ```

7. Open your browser and go to `http://127.0.0.1:8000/` to see the application.

## Usage

- Users can sign up, log in, and create tickets.
- Admins can log in to the Django admin interface at `http://127.0.0.1:8000/admin/` to manage tickets and users.
- Ticket status updates will be communicated via email notifications.
