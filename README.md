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

### Staff View:
- Description: Highlights the view for support staff, where they can access all submitted tickets. Staff can filter tickets by status, add comments, and update ticket statuses to track progress.

https://github.com/user-attachments/assets/1dfde821-13e7-40c2-a637-fd0213e4eb1d

### User Ticket View:
- Description: This view shows how a regular user would create an account, login, and what their home page looks like. Users can track the status of their tickets, add replies, and view responses from the support team.

https://github.com/user-attachments/assets/804119a7-26e9-44a8-a163-b72057744a2a

### Create New Ticket:
- Description: Demonstrates the form users can use to create a new ticket. It includes fields for the ticket title, urgency level, type, and detailed description.

https://github.com/user-attachments/assets/9b65086c-e605-4046-a3db-234b989a1313

### Profile Management:
- Description: Displays how users can update their profile information, including their username, email, and profile picture. This feature allows users to keep their information up to date.

https://github.com/user-attachments/assets/917d2493-5492-4fe7-ba50-948ff49002d7

### Admin View:
- Description: Shows the admin dashboard with full access to all tickets and user profiles. Admins can manage user accounts, view ticket statistics, and oversee the entire ticketing system.

https://github.com/user-attachments/assets/fc756902-8273-42a9-89f9-7ae84ef0c97e

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

