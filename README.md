# Curriculum Management System

A web-based **Curriculum Management System** designed to simplify, digitize, and manage academic curriculum and syllabus-related processes within an educational institution.

The system provides a centralized platform for managing curriculum structures, schemes, courses, electives, syllabus information, booklet generation, dashboards, and academic progress.

## Overview

Managing academic curriculum manually can involve multiple documents, spreadsheets, approvals, and disconnected workflows. This project aims to provide a structured digital system where curriculum-related information can be created, updated, reviewed, and managed from a centralized platform.

The system includes dedicated functionality for curriculum and scheme management along with dashboards and academic workflow support.

## Key Features

### Curriculum & CDC Management

- Dynamic curriculum and CDC structure management
- Curriculum scheme definition and modification
- Course and subject management
- Curriculum structure organization
- Integration between CDC and elective pools
- Dynamic scheme selection

### Elective Management

- Elective pool management
- CDC-to-elective-pool selection
- Dynamic elective allocation
- Structured management of elective subjects

### Syllabus & Scheme Management

- Syllabus structure management
- Scheme definition and improvement
- Academic scheme organization
- Syllabus-related administrative workflows

### Booklet Generation

- Automated curriculum/scheme booklet generation
- Improved booklet generation workflow
- Structured academic information for booklet preparation

### Dashboards

- Role-based dashboard structure
- Academic progress tracking
- Pipeline and workflow tracking
- Centralized overview of curriculum-related activities

## System Architecture

The application follows a modular web application architecture built around the Laravel framework.

```text
                    ┌──────────────────────────┐
                    │       Web Interface       │
                    │      Blade / JavaScript   │
                    └────────────┬─────────────┘
                                 │
                                 ▼
                    ┌──────────────────────────┐
                    │     Laravel Application   │
                    │                          │
                    │ Controllers              │
                    │ Services                 │
                    │ Models                   │
                    │ Routes                   │
                    └────────────┬─────────────┘
                                 │
                ┌────────────────┴────────────────┐
                ▼                                 ▼
       ┌──────────────────┐              ┌──────────────────┐
       │    Database      │              │  File Generation │
       │                  │              │                  │
       │ Curriculum       │              │ Booklets         │
       │ Schemes          │              │ Documents        │
       │ Courses          │              │ Reports          │
       │ Electives        │              │                  │
       └──────────────────┘              └──────────────────┘
```

## Technology Stack

| Layer | Technology |
|---|---|
| Backend | Laravel / PHP |
| Frontend | Blade, JavaScript, CSS |
| Database | Relational Database |
| Package Management | Composer |
| Frontend Build Tool | Vite |
| Testing | PHPUnit |
| Version Control | Git / GitHub |

## Project Structure

```text
Curriculum-Management-system/
│
├── app/
│   ├── Http/
│   ├── Models/
│   └── Services/
│
├── bootstrap/
├── config/
├── database/
│   ├── migrations/
│   └── seeders/
│
├── public/
├── resources/
│   ├── views/
│   ├── css/
│   └── js/
│
├── routes/
├── storage/
├── tests/
│
├── artisan
├── composer.json
├── package.json
└── vite.config.js
```

## Core Modules

The project currently focuses on the following major areas:

- **CDC / Curriculum Management**
- **Scheme Management**
- **Course Management**
- **Elective Pool Management**
- **Syllabus Management**
- **Booklet Generation**
- **Dashboard Management**
- **Academic Progress Tracking**
- **Workflow / Pipeline Management**

## Installation

### Prerequisites

Make sure the following are installed:

- PHP
- Composer
- Node.js and npm
- A supported relational database
- Git

### Clone the Repository

```bash
git clone https://github.com/rishihake-21/Curriculum-Management-system.git
cd Curriculum-Management-system
```

### Install PHP Dependencies

```bash
composer install
```

### Install Frontend Dependencies

```bash
npm install
```

### Environment Configuration

Create the environment file:

```bash
cp .env.example .env
```

On Windows, you can copy `.env.example` to `.env` manually.

Configure the database and other required environment variables in `.env`.

Generate the Laravel application key:

```bash
php artisan key:generate
```

### Database Setup

Run migrations:

```bash
php artisan migrate
```

If the project requires seed data:

```bash
php artisan db:seed
```

### Build Frontend Assets

For development:

```bash
npm run dev
```

For production:

```bash
npm run build
```

### Start the Application

```bash
php artisan serve
```

The application will normally be available at:

```text
http://127.0.0.1:8000
```

## Development Workflow

A typical development workflow is:

```text
Requirement
     ↓
Curriculum / Scheme Design
     ↓
Database Structure
     ↓
Backend Logic
     ↓
Dashboard / UI
     ↓
Testing
     ↓
Booklet / Document Generation
     ↓
Academic Review
```

## Project Goals

The main goals of the system are to:

- Digitize curriculum management workflows
- Reduce manual curriculum-related work
- Centralize academic curriculum information
- Improve scheme and syllabus management
- Simplify elective management
- Improve visibility through dashboards
- Support automated academic document generation
- Provide a structured platform for future ERP integration

## Future Scope

Potential future enhancements include:

- Integration with an institutional ERP/UMS
- Advanced role-based access control
- Approval workflows for curriculum changes
- Version control for curriculum schemes
- Advanced academic analytics
- Notification and communication systems
- Improved reporting
- API-based integration with other academic systems
- Audit logs for curriculum modifications

## Project Status

The system is under active development.

Current development focuses on improving:

- Curriculum/CDC workflows
- Dynamic scheme management
- Elective pool integration
- Dashboard functionality
- Academic progress tracking
- Booklet generation

## License

This project is developed for academic and institutional use.

---

## Author

**Rushikesh Hake**

Computer Technology Student

GitHub: [@rishihake-21](https://github.com/rishihake-21)
