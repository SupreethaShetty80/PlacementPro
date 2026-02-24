# PlacementPro - The Integrated Campus Career Suite

PlacementPro is a comprehensive web-based placement management system designed to automate and streamline the entire campus placement process. Built with Flask, it replaces traditional Excel sheets and notice boards with a dynamic, role-based platform connecting TPOs, Students, and Alumni.

##  Key Features

###  For TPOs (Admin)
- **Criteria Engine**: Create drives with eligibility criteria (CGPA, backlogs, branches) and instantly filter eligible students
- **One-Click Notifications**: Send bulk email notifications to eligible students using Flask-Mail
- **Interview Scheduler**: Drag-drop calendar for slot booking with conflict prevention
- **Analytics Dashboard**: Track placement statistics and student progress

###  For Students
- **Resume Wizard**: Generate standardized PDF resumes instantly using ReportLab
- **Personalized Job Feed**: View only eligible drives based on profile
- **Application Tracker**: Real-time status updates (Applied → Shortlisted → Selected)
- **Skill Gap Analysis**: Compare skills against market requirements

###  For Alumni
- **Job Referral Board**: Post job openings from current companies
- **Mentorship Slots**: Set available hours for student guidance
- **Industry Connect**: Give back to alma mater

##  Tech Stack

- **Backend**: Flask 2.3.x (Python)
- **Database**: SQLite with SQLAlchemy ORM
- **Authentication**: Flask-Login (Role-based access)
- **PDF Generation**: ReportLab
- **Email Service**: Flask-Mail
- **Frontend**: Bootstrap 5, Jinja2, Chart.js
- **Scheduler**: FullCalendar.io integration

## 📋 Prerequisites

- Python 3.9+
- pip package manager
- Virtual environment (recommended)

## 🚀 Installation

```bash
# Clone repository
git clone https://github.com/SupreethaShetty80/placementpro.git
cd placementpro

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt

# Set environment variables
cp .env.example .env
# Edit .env with your credentials

# Run application
python run.py
