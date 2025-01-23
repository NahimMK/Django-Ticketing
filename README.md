# Django Ticketing

A **ticketing system** built with Django and Python, designed to allow users to create, manage, and track support tickets. This system differentiates between regular users, tech support, and admins, offering a tailored view and functionality based on user roles.

---

## Table of Contents

1. [Features](#features)
   - [For Regular Users](#for-regular-users)
   - [For Tech Support Team](#for-tech-support-team)
   - [For Admins](#for-admins)
2. [Screen Recordings](#screen-recordings)
3. [Installation](#installation)
4. [Technologies Used](#technologies-used)
5. [Ticket Filtering and Sorting](#ticket-filtering-and-sorting)
6. [Challenges Faced](#challenges-faced)
7. [Future Improvements](#future-improvements)
8. [Contributing](#contributing)
9. [License](#license)

---

## Features

### For Regular Users:
- **Submit New Tickets**: Users can create tickets with a title, urgency level, and detailed description.
- **View Own Tickets**: Users can only see tickets they have created.
- **Reply to Tickets**: Users can reply to tickets to provide updates or ask questions.

### For Tech Support Team:
- **Access All Tickets**: Tech support staff can view and manage all user-submitted tickets.
- **Update Ticket Status**: Tech support can change ticket statuses (e.g., New, Open, Working, Closed).
- **Add Replies**: Tech support can comment on tickets to communicate with users or add progress updates.
- **Filter and Sort Tickets**: Tech support can filter tickets based on their status (New, Open, Working, Closed) to quickly locate and address specific tickets. Sorting options by urgency or creation date are also available.

### For Admins:
- **Full Access**: Admins can see and manage all tickets and user profiles.
- **User Management**: Admins have additional rights for managing user data and accounts.
- **Dashboard Overview**: Admins can view a summary of ticket activity, including the number of tickets in each status, average resolution time, and more.

---

## Screen Recordings

### User Ticket View:
![User Ticket View](https://github.com/user-attachments/assets/f93a76ac-d222-4e2c-b933-4dbdee682960)

### Create New Ticket:
![Create New Ticket](https://github.com/user-attachments/assets/c8284a8c-c2b7-464f-91c7-40885e1b7384)

### Profile Management:
![Profile Management](https://github.com/user-attachments/assets/00899733-6147-447d-bc35-13baa8f82c8f)

### Staff View:
![Login Page](https://github.com/user-attachments/assets/b3cb3643-698e-4ece-b77b-473fb43406ae)

### Admin View:
![Login Page](https://github.com/user-attachments/assets/998b3c2a-6664-4b2c-8ea1-48a2480e4b3b)


---

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/NahimMK/Django-Ticketing.git
   cd Django-Ticketing
   ```

2. **Set Up a Virtual Environment** (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply Migrations**:
   ```bash
   python manage.py migrate
   ```

5. **Create a Superuser**:
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the Development Server**:
   ```bash
   python manage.py runserver
   ```

7. **Access the Application**:
   - Open your browser and go to: [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

---

## Technologies Used

- **Backend**: Django (Python)
- **Frontend**: Django templates and Bootstrap for styling.
- **Database**: SQLite (default for Django; easily configurable for PostgreSQL or MySQL).

---

## Ticket Filtering and Sorting

The ticketing system includes robust filtering and sorting functionality to improve workflow efficiency:

- **Filter Options**:
  - **New Tickets**: View tickets that have just been submitted and require review.
  - **Open Tickets**: View tickets that are actively being worked on.
  - **Working Tickets**: See tickets currently in progress.
  - **Closed Tickets**: Quickly find tickets that have been resolved.

- **Sorting Options**:
  - Sort tickets by **urgency level** to address the most critical issues first.
  - Sort by **creation date** to prioritize older tickets that need attention.

---

## Challenges Faced

- **Dependency Management**: Resolving conflicts between updated versions of libraries and ensuring compatibility.
- **Role-Based Views**: Implementing access control to differentiate between regular users, tech support, and admins. Each role required different permissions and UI views.
- **Filtering and Sorting Logic**: Designing an intuitive system for filtering and sorting tickets required thoughtful planning and testing.
- **Scalability**: Ensuring that the application can handle a large number of tickets and users without performance degradation.

---

## Future Improvements

1. **Enhanced Search and Filter Options**:
   - Add advanced search functionality to find tickets by keywords, usernames, or tags.

2. **Email Notifications**:
   - Notify users via email when their ticket status changes or when a reply is added.

3. **Mobile Responsiveness**:
   - Optimize the interface for mobile devices to ensure usability across all platforms.

4. **Dashboard Analytics**:
   - Provide admins and tech support with statistics on ticket volume, average resolution time, most common issues, etc.

5. **Integration with External Tools**:
   - Allow ticket export to tools like Excel or integration with third-party project management systems.

---

## Contributing

Contributions are welcome! If you’d like to improve this project, feel free to fork the repository and submit a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/NahimMK/Django-Ticketing/blob/main/LICENSE) file for details.

---

### requirements.txt
```plaintext
asgiref>=3.6.0,<4
distlib==0.3.4
Django==4.2
django-crispy-forms==1.14.0
django-guardian==2.4.0
filelock==3.7.1
platformdirs==2.5.2
six==1.16.0
sqlparse==0.4.2
tzdata==2022.1
virtualenv==20.15.1
```

