
# 🦷 Dental Clinic Management System

[![Dental Clinic Management System][(docs/thumbnail.png)](https://github.com/Vimal4hckr/Dental-management-repo/blob/main/nir's%20banner.png)](https://github.com/Vimal4hckr/Dental-management-repo/blob/main/nir's%20banner.png)

A modern, full-featured **Dental Clinic Management System** built with **Django** and designed to digitize and simplify the complete workflow of a dental clinic.

The system provides dedicated, role-based functionality for **Administrators, Dentists, Receptionists/Staff, and Patients**, covering appointment management, patient records, dental charts, treatments, prescriptions, billing, inventory, reviews, analytics, and AI-assisted tools.

The application also includes a modern public-facing website and a custom management panel for clinic administration.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [User Roles](#-user-roles)
- [Tech Stack](#-tech-stack)
- [System Architecture](#-system-architecture)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Database Configuration](#-database-configuration)
- [Demo Accounts](#-demo-accounts)
- [Key URLs](#-key-urls)
- [AI Features](#-ai-features)
- [Static Files](#-static-files)
- [Deployment](#-deployment)
- [Testing](#-testing)
- [Security](#-security)
- [Future Enhancements](#-future-enhancements)
- [License](#-license)

---

# 📌 Overview

The Dental Clinic Management System is designed to provide a centralized platform for managing the daily operations of a modern dental practice.

Instead of maintaining separate records for appointments, patients, treatments, prescriptions, billing, and inventory, the system brings these workflows together into a single web application.

### The system supports:

- 👨‍💼 Administrator management
- 🧑‍⚕️ Dentist/Doctor operations
- 🧑‍💼 Receptionist/Staff operations
- 🧑 Patient services
- 📅 Appointment management
- 🦷 Interactive dental/tooth chart
- 📝 Clinical treatment records
- 💊 Digital prescriptions
- 💰 Billing and invoices
- 📦 Inventory management
- ⭐ Patient reviews
- 🤖 Offline AI-assisted tools
- 📊 Clinic analytics
- 🌐 Public clinic website
- 🔐 Role-based authentication and authorization

---

# ✨ Features

## 👨‍💼 Administrator Dashboard

The administrator has complete control over the clinic management system.

### Capabilities

- Manage doctors/dentists
- Manage receptionists/staff
- Manage patients
- Manage appointments
- Manage clinic services
- Manage treatments
- Manage invoices
- Manage inventory
- Manage reviews
- View clinic statistics
- View revenue information
- View appointment analytics
- Manage system records
- Role-based access control

---

## 🧑‍⚕️ Dentist / Doctor Dashboard

The dentist dashboard focuses on clinical operations and patient care.

### Capabilities

- View appointments
- View patient information
- View patient history
- Manage treatment records
- Record diagnosis
- Manage dental/tooth conditions
- Add treatment information
- Create prescriptions
- View previous prescriptions
- Track treatment costs
- Update appointment status
- Access patient clinical information

---

## 🧑‍💼 Receptionist / Staff Dashboard

The receptionist/staff interface focuses on front-desk and clinic operations.

### Capabilities

- Register patients
- Manage patient information
- Book appointments
- Manage appointment schedules
- View dentist availability
- Update appointment status
- Manage patient visits
- Manage billing-related information
- Assist with clinic administration

---

## 🧑 Patient Dashboard

Patients can access their own clinic-related information through a dedicated dashboard.

### Capabilities

- Patient registration/login
- Manage personal profile
- View appointments
- Book appointments
- Track appointment status
- View treatment information
- View prescriptions
- View dental history
- View billing information
- Submit reviews/feedback

---

# 🦷 Dental / Tooth Chart

The system provides an interactive dental chart for maintaining tooth-level clinical information.

### Supported functionality

- Universal tooth numbering
- Individual tooth selection
- Tooth condition tracking
- Patient-specific dental records
- Treatment association
- Clinical history

This allows dentists to maintain a structured digital representation of a patient's dental condition.

---

# 📅 Appointment Management

The appointment module allows clinic staff and patients to manage appointments efficiently.

### Appointment statuses

- Pending
- Confirmed
- Completed
- Cancelled
- No-Show

The system maintains appointment information including:

- Patient
- Dentist
- Appointment date
- Appointment time
- Status
- Treatment/service
- Additional information

---

# 💊 Digital Prescriptions

Dentists can create and manage digital prescriptions.

### Features

- Multiple medicines per prescription
- Medicine name
- Dosage
- Frequency
- Duration
- Instructions
- Printable prescription view
- Patient prescription history

---

# 💰 Billing & Invoicing

The billing module helps clinics maintain structured financial records.

### Features

- Invoice generation
- Invoice line items
- Service/treatment charges
- Quantity
- Tax
- Discounts
- Partial payments
- Payment tracking
- Automatic balance calculation
- Invoice status

---

# 📦 Inventory Management

The inventory module helps track clinic supplies and medicines.

### Features

- Product/item management
- Stock quantity
- Stock updates
- Low-stock monitoring
- Inventory records
- Product information

---

# ⭐ Reviews & Feedback

Patients can provide feedback about their clinic experience.

Reviews can be managed through the administration panel and displayed on the public website where appropriate.

---

# 🤖 Offline AI Tools

The project includes lightweight, **rule-based AI-assisted tools** that work without external AI APIs.

No OpenAI API key or paid AI service is required for these features.

### Available tools

#### 🩺 Symptom Checker

Provides rule-based informational guidance based on entered symptoms.

#### 💬 Dental Chatbot

Provides predefined/rule-based responses to common dental-related questions.

#### 💰 Treatment Cost Estimator

Provides estimated treatment costs based on selected services and available pricing information.

#### 📊 No-Show Risk

Provides a rule-based estimation of appointment no-show risk.

> ⚠️ These tools are intended for informational and demonstration purposes only and are not a substitute for professional medical diagnosis or treatment.

---

# 📊 Analytics & Dashboard

The system provides visual analytics for clinic management.

### Examples

- Total patients
- Total appointments
- Completed appointments
- Pending appointments
- Revenue
- Patient growth
- Appointment statistics
- Inventory information

Charts can be displayed using **Chart.js**.

---

# 🌐 Public Website

The project also includes a public-facing dental clinic website.

### Public pages include:

- Home
- Services
- About
- Contact
- Service pricing
- Clinic information
- Patient reviews

The public website is designed to provide patients with information before logging into the management system.

---

# 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| Programming Language | Python |
| Backend Framework | Django 5.x |
| Architecture | MVT |
| Database - Development | SQLite |
| Database - Production | PostgreSQL |
| Frontend | HTML5, CSS3, JavaScript |
| UI Framework | Bootstrap 5 |
| Icons | Bootstrap Icons |
| Charts | Chart.js |
| Image Processing | Pillow |
| Database Driver | psycopg2-binary |
| Database Configuration | dj-database-url |
| Static Files | WhiteNoise |
| Production Server | Gunicorn |
| Deployment | Render |
| Version Control | Git & GitHub |

---

# 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │     Public Website  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Django Web App    │
                    └──────────┬──────────┘
                               │
          ┌────────────────────┼────────────────────┐
          │                    │                    │
          ▼                    ▼                    ▼
   Authentication        Clinic Management     AI Assistant
          │                    │                    │
          │          ┌─────────┼─────────┐          │
          │          │         │         │          │
          ▼          ▼         ▼         ▼          ▼
       Admin      Patients  Doctors  Billing    AI Tools
                     │         │
                     └────┬────┘
                          │
                          ▼
                  ┌─────────────────┐
                  │   PostgreSQL    │
                  │    Database     │
                  └─────────────────┘
````

---

# 👥 User Roles

| Role                 | Main Responsibilities                                        |
| -------------------- | ------------------------------------------------------------ |
| Administrator        | Complete clinic and system management                        |
| Dentist / Doctor     | Patient care, treatments and prescriptions                   |
| Receptionist / Staff | Patients, appointments and front-desk operations             |
| Patient              | Appointments, treatments, prescriptions and personal records |

Each role receives access only to the features relevant to its responsibilities.

---

# 📁 Project Structure

```text
Dental-management-repo/
│
├── dental_clinic/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
│
├── accounts/
│   ├── migrations/
│   ├── templates/
│   ├── admin.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
│
├── clinic/
│   ├── migrations/
│   ├── templates/
│   ├── admin.py
│   ├── models.py
│   ├── urls.py
│   └── views.py
│
├── pages/
│   ├── templates/
│   ├── urls.py
│   └── views.py
│
├── aiassistant/
│   ├── migrations/
│   ├── templates/
│   ├── urls.py
│   └── views.py
│
├── manage_panel/
│   ├── migrations/
│   ├── templates/
│   ├── urls.py
│   └── views.py
│
├── templates/
│   └── base.html
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
├── media/
│
├── docs/
│   └── thumbnail.png
│
├── report/
│   └── diagrams/
│
├── manage.py
├── requirements.txt
├── .gitignore
└── README.md
```

---

# 🚀 Getting Started

## Prerequisites

Make sure the following are installed:

* Python 3.10+
* pip
* Git
* PostgreSQL (for production/local PostgreSQL setup)

Check Python:

```bash
python --version
```

Check pip:

```bash
pip --version
```

---

# 1️⃣ Clone the Repository

```bash
git clone https://github.com/Vimal4hckr/Dental-management-repo.git
```

Move into the project:

```bash
cd Dental-management-repo
```

---

# 2️⃣ Create Virtual Environment

### Windows

```bash
python -m venv venv
```

Activate:

```bash
venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv venv
```

Activate:

```bash
source venv/bin/activate
```

---

# 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 4️⃣ Configure Environment Variables

Create a `.env` file for local development if your configuration uses environment variables.

Example:

```env
SECRET_KEY=your-secret-key
DEBUG=True
DATABASE_URL=postgresql://username:password@localhost:5432/dental_clinic
```

For production:

```env
SECRET_KEY=your-production-secret-key
DEBUG=False
DATABASE_URL=your-production-database-url
```

> Never commit `.env` files or database credentials to GitHub.

---

# 5️⃣ Run Database Migrations

```bash
python manage.py makemigrations
```

Then:

```bash
python manage.py migrate
```

---

# 6️⃣ Create Superuser

Create an administrator account:

```bash
python manage.py createsuperuser
```

Enter the requested username, email and password.

---

# 7️⃣ Collect Static Files

For production:

```bash
python manage.py collectstatic --noinput
```

---

# 8️⃣ Run the Development Server

```bash
python manage.py runserver
```

Open:

```text
http://127.0.0.1:8000/
```

---

# 🔐 Environment Variables

The production deployment requires the following environment variables:

| Variable       | Description                        |
| -------------- | ---------------------------------- |
| `SECRET_KEY`   | Django secret key                  |
| `DEBUG`        | Django debug mode                  |
| `DATABASE_URL` | PostgreSQL database connection URL |

### Example

```env
SECRET_KEY=your-secret-key
DEBUG=False
DATABASE_URL=postgresql://user:password@host:5432/database
```

---

# 🗄️ Database Configuration

The project supports different databases depending on the environment.

### Development

```text
SQLite
```

### Production

```text
PostgreSQL
```

The production database is configured through:

```env
DATABASE_URL
```

For Render deployment, use the **Internal Database URL** provided by the Render PostgreSQL database when the web service and database are in the same Render environment/region.

---

# 🔑 Demo Accounts

If demo/seed data is available in the current project, the following role structure can be used for testing:

| Role          | Username    | Password                |
| ------------- | ----------- | ----------------------- |
| Administrator | `admin`     | Configured during setup |
| Dentist       | `doctor`    | Configured during setup |
| Receptionist  | `reception` | Configured during setup |
| Patient       | `patient`   | Configured during setup |

> Update these credentials according to the accounts configured in the database. Never expose real production credentials in this README.

---

# 🔗 Key URLs

| URL          | Description                              |
| ------------ | ---------------------------------------- |
| `/`          | Public homepage                          |
| `/accounts/` | Authentication and account functionality |
| `/app/`      | Clinic management application            |
| `/ai/`       | AI assistant features                    |
| `/manage/`   | Custom management panel                  |

### Main application areas

```text
/
├── Public Website
│
├── accounts/
│   └── Authentication
│
├── app/
│   └── Clinic Management
│
├── ai/
│   └── AI Assistant
│
└── manage/
    └── Management Panel
```

---

# 🎨 User Interface

The application provides separate interfaces for different user roles.

### Administrator

```text
Dashboard
├── Users
├── Doctors
├── Receptionists
├── Patients
├── Appointments
├── Services
├── Billing
├── Inventory
└── Reports
```

### Dentist

```text
Dashboard
├── Appointments
├── Patients
├── Dental Chart
├── Treatments
├── Prescriptions
└── Patient History
```

### Receptionist

```text
Dashboard
├── Patients
├── Appointments
├── Doctors
├── Services
└── Billing
```

### Patient

```text
Dashboard
├── Profile
├── Appointments
├── Treatments
├── Prescriptions
├── Dental History
└── Reviews
```

---

# 🚀 Deployment on Render

The project is configured for deployment using **Render**.

## Build Command

```bash
pip install -r requirements.txt && python manage.py migrate && python manage.py collectstatic --noinput
```

## Start Command

```bash
gunicorn dental_clinic.wsgi:application
```

## Environment Variables

Configure these in the Render Web Service:

```text
SECRET_KEY
DEBUG=False
DATABASE_URL
```

### Render PostgreSQL

Create a PostgreSQL database on Render and connect it to the Django web service using:

```text
DATABASE_URL
```

When both services are hosted within the same Render environment/region, prefer the database's **Internal Database URL**.

---

# 🔄 Production Deployment Flow

```text
                 GitHub
                    │
                    ▼
             Render Web Service
                    │
                    ▼
          pip install requirements
                    │
                    ▼
             Django Migrations
                    │
                    ▼
            Collect Static Files
                    │
                    ▼
                 Gunicorn
                    │
                    ▼
            Django Application
                    │
                    ▼
              PostgreSQL
```

---

# 📦 Production Dependencies

The production environment uses packages including:

```text
Django
gunicorn
psycopg2-binary
dj-database-url
whitenoise
Pillow
```

Install all dependencies with:

```bash
pip install -r requirements.txt
```

---

# 🧪 Testing & Validation

Before deployment, run Django's system checks:

```bash
python manage.py check
```

Run migrations:

```bash
python manage.py migrate
```

Run tests:

```bash
python manage.py test
```

You can also verify the production configuration using:

```bash
python manage.py check --deploy
```

---

# 🔒 Security

The application follows common Django security practices.

### Sensitive information should never be committed:

* `.env`
* Database passwords
* `SECRET_KEY`
* API keys
* Production credentials
* Private configuration files

Example `.gitignore`:

```gitignore
.env
venv/
.venv/
__pycache__/
*.pyc
db.sqlite3
staticfiles/
media/
```

### Production recommendations

```text
DEBUG=False
Strong SECRET_KEY
Secure database credentials
HTTPS
Secure cookies
CSRF protection
Role-based permissions
```

---

# 📈 Future Enhancements

Possible future improvements include:

* 📱 Dedicated mobile application
* 📲 WhatsApp appointment notifications
* 📧 Email notifications
* 💳 Online payment integration
* 📅 Advanced appointment scheduling
* 🦷 Advanced dental treatment chart
* 📄 PDF prescription generation
* 🧾 Professional invoice PDF generation
* 📊 Advanced business analytics
* 📦 Automated inventory alerts
* 🔔 Appointment reminders
* ☁️ Cloud document storage
* 🧠 Advanced AI assistant
* 🗣️ Voice-based patient assistant
* 🔐 Two-factor authentication
* 📱 Progressive Web App support

---

# 🏥 Intended Use

This project can be customized according to the workflow and requirements of an individual dental clinic.

Possible customization areas include:

* Clinic branding
* Dentist profiles
* Services
* Treatment pricing
* Appointment workflow
* Billing structure
* Prescription format
* Patient registration
* Dental chart
* Reports
* User permissions

---

# 📚 Documentation

Additional documentation and project diagrams can be maintained inside:

```text
docs/
report/
report/diagrams/
```

Recommended project documentation includes:

* System Architecture
* Use Case Diagram
* ER Diagram
* Data Flow Diagram
* Class Diagram
* Sequence Diagram
* Activity Diagram
* Database Design
* Module Documentation
* User Manual

---

# ⚠️ Medical Disclaimer

The AI-assisted features included in this project are **rule-based informational tools** intended for educational and demonstration purposes.

They should not be used as a replacement for:

* Professional dental diagnosis
* Clinical examination
* Medical treatment
* Emergency medical care
* Professional dental advice

Patients should always consult a qualified dental professional for medical decisions.

---

# 📄 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for more information.

---

# 👨‍💻 Development

Developed as a complete **Django-based Dental Clinic Management System** with a focus on:

* Clean architecture
* Role-based access
* Modern UI
* Clinic workflow automation
* Database-driven management
* Offline AI-assisted functionality
* Production deployment

---

## 🦷 Dental Clinic Management System

**Django • PostgreSQL • Bootstrap • JavaScript • Chart.js • Gunicorn • Render**

> Built to provide a centralized, scalable and modern digital management platform for dental clinics.

````

### One important correction for your current project

Since you are deploying **your customized `Dental-management-repo`**, don't copy the original README's:

```text
git clone https://github.com/sumitkumar1503/Dental-Clinic-Management-System.git
````

I changed it to your repository:

```bash
git clone https://github.com/Vimal4hckr/Dental-management-repo.git
```

And I also **didn't hard-code the old demo passwords** from the reference README, because those may not match your current database.

For your current Render setup, the most important production section is:

```text
Build Command:
pip install -r requirements.txt && python manage.py migrate && python manage.py collectstatic --noinput

Start Command:
gunicorn dental_clinic.wsgi:application

Database:
PostgreSQL

DATABASE_URL:
Render PostgreSQL → Internal Database URL
```

This README is suitable for putting directly into the repository as `README.md`.
