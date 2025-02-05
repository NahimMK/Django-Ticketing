# Django Ticketing System | Cloud-Based Issue Tracker

A scalable, cloud-hosted ticketing system designed to streamline issue tracking and support management.  
This system allows users to create and track tickets, tech support to resolve them, and admins to oversee operations using role-based access control (RBAC).

The system is deployed on AWS EC2, secured with SSL & AWS Security Groups, and automated using Docker & CI/CD pipelines.

---

## Why This Project Matters
- **Full-Stack Development:** Built with Django, PostgreSQL, and Bootstrap for a responsive UI.  
- **Cloud Deployment:** Deployed on AWS EC2, with Nginx & Gunicorn for production.  
- **DevOps & CI/CD:** Automated using Docker, GitHub Actions, and Let's Encrypt SSL.  
- **Scalable & Secure:** Implements RBAC, cloud security best practices, and efficient database management.  

---

## Features

### User Role: Regular Users
- Submit, track, and update support tickets.
- View ticket history and communicate with support teams.

### User Role: Tech Support
- View and manage all submitted tickets.
- Assign statuses (New, Open, Working, Closed).
- Communicate with users and add internal notes.

### User Role: Admins
- Manage users, roles, and permissions.
- Monitor ticket status and resolution progress.
- Oversee system security settings and configurations.

---

## Tech Stack & Cloud Deployment

| Category | Technologies Used |
|----------|------------------|
| **Backend** | Django (Python) |
| **Frontend** | Django Templates, Bootstrap |
| **Database** | PostgreSQL (Docker) |
| **Cloud Provider** | AWS (EC2, Route 53, RDS, S3) |
| **DevOps & CI/CD** | GitHub Actions, Docker, Nginx, Gunicorn |

---

## Live Demo
- **URL:** [nahim-django-ticketing.com](https://nahim-django-ticketing.com)  
- **Security:** Secured with Let's Encrypt SSL & AWS Security Groups  

---

## Video Walkthrough

https://github.com/user-attachments/assets/9559cc53-b395-4866-acc9-a0d47028cd52

---

## Project Impact
This project demonstrates expertise in cloud computing, full-stack development, and DevOps:
- Implements user authentication and ticket management with Django’s built-in features.
- Optimized for scalability and security using Nginx, Gunicorn, and PostgreSQL.
- Deployed on AWS EC2 with Docker, enabling containerized scalability.
- Secured with HTTPS & AWS security configurations, ensuring safe user interactions.
- Automated CI/CD pipeline with GitHub Actions, enabling quick updates & reliability.

---

## Installation & Setup (Local)
Clone the repo and set up the project locally:

```bash
git clone https://github.com/NahimMK/Django-Ticketing.git
cd Django-Ticketing
```

### 1. Create a Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scriptsctivate
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Apply Migrations & Create Superuser
```bash
python manage.py migrate
python manage.py createsuperuser
```

### 4. Run the Development Server
```bash
python manage.py runserver
```
Visit: **[http://127.0.0.1:8000/](http://127.0.0.1:8000/)**

---

## Cloud Deployment (AWS)

### 1. Deploy with Docker & AWS EC2
```bash
docker-compose up -d --build
```

### 2. Setup Nginx & Gunicorn for Production
```bash
sudo systemctl restart nginx
```

### 3. Secure with SSL (Let’s Encrypt)
```bash
sudo certbot --nginx -d nahim-django-ticketing.com -d www.nahim-django-ticketing.com
```

---

## Filtering & Sorting Features
- Filter by Status: New, Open, Working, Closed.
- Sort by Urgency & Creation Date.

---

## Challenges & Solutions

| Challenge | Solution Implemented |
|-----------|----------------------|
| Role-Based Access Control | Used Django Guardian for fine-grained user permissions. |
| Secure Cloud Deployment | Configured AWS Security Groups and Let’s Encrypt SSL. |
| Automating Deployment | Integrated GitHub Actions (CI/CD) for auto-deployment. |

---

## Future Enhancements
- Email Notifications for ticket updates.
- Admin Dashboard Analytics for deeper insights.
- Mobile-Responsive UI for a better user experience.

---

## Contact

- **Email:** [nahimmdk@gmail.com](mailto:nahimmdk@gmail.com)  
- **LinkedIn:** [linkedin.com/in/nahim-mk](https://linkedin.com/in/nahim-mk)  
- **GitHub:** [github.com/NahimMK](https://github.com/NahimMK)  

---


## Acknowledgments
Thanks to AWS and Django for their free tier services.
