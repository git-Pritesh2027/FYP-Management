# FYP-Management
A web-based FYP Management System built with React, Django REST Framework, and PostgreSQL to streamline project submissions, supervisor coordination, progress tracking, and academic workflows.  Topics/Tags: `react` `django` `django-rest-framework` `postgresql` `fyp-management` `jwt-authentication`


# FYP Management System

A web-based platform designed to simplify and organize the Final Year Project (FYP) process for students, teachers, and administrators. The system aims to manage project proposals, supervisor allocation, project progress, submissions, and academic coordination through a centralized platform.

## Overview

Managing final-year projects manually can lead to communication gaps, scattered documents, missed deadlines, and difficulties tracking project progress.

The **FYP Management System** aims to address these challenges by providing a centralized workspace where students can manage their projects, supervisors can monitor progress, and administrators can oversee the overall project workflow.

## Objectives

* Simplify final-year project management and coordination.
* Organize project proposals, submissions, and deadlines.
* Enable supervisors to review and monitor student progress.
* Provide role-based access for students, teachers, and administrators.
* Maintain project-related information in a centralized database.
* Improve transparency and reduce manual coordination.

## User Roles

### 1. Administrator

* Manage students, teachers, and project-related records.
* Oversee project allocation and academic workflows.
* Monitor project progress and submission status.

### 2. Teacher / Supervisor

* View assigned student projects.
* Review project proposals and submissions.
* Monitor progress and provide feedback.
* Track project milestones and deadlines.

### 3. Student

* View project-related information.
* Submit project proposals and required documents.
* Track project progress and deadlines.
* View supervisor feedback and submission status.

*Note: Features will be available according to the implementation and configured permissions.*

## Technology Stack

| Component      | Technology               |
| -------------- | ------------------------ |
| Frontend       | React.js                 |
| Build Tool     | Vite                     |
| Backend        | Python, Django           |
| API Framework  | Django REST Framework    |
| Database       | PostgreSQL               |
| Authentication | JWT-based authentication |
| Communication  | REST APIs                |

## System Architecture

The application follows a frontend-backend architecture.

* **Frontend:** Provides the user interface and communicates with the backend through API requests.
* **Backend:** Handles business logic, authentication, permissions, and project workflows.
* **Database:** PostgreSQL stores application data.
* **API Layer:** Django REST Framework exposes endpoints under `/api/v1/`.

## Project Structure

```text
fyp-management-system/
├── frontend/          # React + Vite application
├── backend/           # Django REST Framework application
├── docs/              # Project documentation
│   ├── PRD.md
│   ├── RULES.md
│   ├── ARCHITECTURE.md
│   ├── DESIGN.md
│   ├── TASK.md
│   ├── MEMORY.md
│   └── PROJECT_CONTEXT.md
└── README.md
```

*The directory structure may evolve as development progresses.*

## Getting Started

### Prerequisites

Install the following before setting up the project:

* Node.js and npm
* Python 3
* PostgreSQL
* Git

### 1. Clone the Repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd fyp-management-system
```

### 2. Set Up the Backend

```bash
cd backend
python -m venv venv
```

Activate the virtual environment.

**Windows:**

```bash
venv\Scripts\activate
```

**Linux / macOS:**

```bash
source venv/bin/activate
```

Install the backend dependencies:

```bash
pip install -r requirements.txt
```

Configure the required environment variables and PostgreSQL database before running migrations.

```bash
python manage.py migrate
python manage.py runserver
```

### 3. Set Up the Frontend

Open a new terminal:

```bash
cd frontend
npm install
npm run dev
```

The frontend and backend configuration may require additional setup as development progresses.

## API Overview

Backend API prefix:

```text
/api/v1/
```

The API will handle authentication, user management, project workflows, submissions, and other application features as they are implemented.

## Documentation

Detailed project documentation is maintained in the `docs/` directory, including:

* **PRD.md:** Product requirements and functional scope.
* **RULES.md:** Development conventions and project rules.
* **ARCHITECTURE.md:** System architecture and component responsibilities.
* **DESIGN.md:** UI/UX design guidelines.
* **TASK.md:** Development tasks and progress.
* **MEMORY.md:** Important implementation decisions.
* **PROJECT_CONTEXT.md:** Project background and context.

## Project Status

**Status:** Under Development

The system is being developed incrementally. Features, setup instructions, and documentation will be updated as implementation progresses.

## Future Enhancements

Potential enhancements include:

* Automated deadline reminders and notifications.
* Project evaluation and review workflows.
* Progress reports and analytics dashboards.
* Exportable project reports.
* Improved document and submission management.

## Contributing

This project is currently being developed as an academic project. Suggestions, feedback, and improvements are welcome.

## License

A license has not yet been selected. All rights are reserved by the repository owner unless a license is added.
