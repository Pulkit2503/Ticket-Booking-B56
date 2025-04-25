Ticket Booking Management System
Project Overview
The Ticket Booking Management System is a web application built using Django. It allows users to view available shows/events, book tickets, and view their booking history. Admins can manage shows (add/edit/delete) and view all bookings through a custom admin panel.

Setup & Run Instructions
Prerequisites
Python 3.10 or higher
Docker and Docker Compose
Jenkins (optional for CI/CD)
Steps
Clone the repository:

git clone <repository-url>
cd ticket_booking
Install dependencies:

pip install -r requirements.txt
Apply migrations:

python manage.py migrate
Run the development server:

python manage.py runserver
Access the application at http://127.0.0.1:8000/.

To populate the database with sample shows, run:

python manage.py populate_shows
Using Docker
Build and run the application:

docker-compose up --build
Access the application at http://127.0.0.1:8000/.

Using Jenkins
Add the repository to Jenkins.
Use the provided Jenkinsfile for CI/CD pipeline configuration.
Tech Stack Used
Backend: Django
Database: SQLite (default), PostgreSQL (via Docker)
Frontend: HTML, CSS
Containerization: Docker, Docker Compose
CI/CD: Jenkins
Notes
Ensure Docker and Docker Compose are installed for containerized deployment.
Use the Jenkinsfile for automated build, test, and deployment pipelines.
