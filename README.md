# Stage 3 - Django Project

## Project Overview
Stage 3 builds upon the previous stages by integrating external services and introducing advanced configurations. This phase focuses on enhancing the application with external APIs and preparing for scalability.

## Repository Structure
```
stage-3/
├── api/                # Contains the API-related files and configurations
├── uninest/            # Core Django project directory
├── client_secret_xxx/  # File for managing external service credentials
├── db.sqlite3          # Default SQLite database file
├── manage.py           # Django management script
├── requirements.txt    # Python dependencies for the project
```

### 1. `api/`
Continues to house the serializers, views, and URLs for the API endpoints. In this stage, endpoints are extended to incorporate external API calls and advanced functionality.

### 2. `uninest/`
The central project directory, with updates to settings and middleware to support external integrations and advanced configurations. 

### 3. `client_secret_xxx`
This file stores credentials for integrating third-party services securely. Ensure this file is not exposed publicly by including it in `.gitignore`.

### 4. `db.sqlite3`
SQLite remains the default database. It now includes data from new features and integrations. Migrating to a more robust database is recommended for production.

### 5. `manage.py`
Remains the entry point for managing Django operations, including migrations, server startup, and application management.

### 6. `requirements.txt`
Updated with additional dependencies for external integrations. Install them using:
```bash
pip install -r requirements.txt
```

## Getting Started
Follow these steps to set up and run the project locally:

### Prerequisites
- Python (>= 3.8)
- pip (Python package manager)

### Installation
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd stage-3
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Configure external service credentials:
   - Ensure the `client_secret_xxx` file is correctly set up with valid credentials.

5. Run database migrations:
   ```bash
   python manage.py migrate
   ```

6. Start the development server:
   ```bash
   python manage.py runserver
   ```

7. Access the application at `http://127.0.0.1:8000/`.

## Key Updates in Stage 3
- Integrated external services via `client_secret_xxx`.
- Enhanced API functionality with external API calls.
- Improved settings and middleware for scalability.
---
Stay tuned for updates in Stage 4!
