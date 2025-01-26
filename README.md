# Flask Application Setup Guide

This guide provides step-by-step instructions to set up a Flask application using a virtual environment, install dependencies, and run the application.

## 1. Create a Virtual Environment
Ensure Python is installed (check with `python3 --version`).

Run the following command to create a virtual environment:

```bash
python3 -m venv venv
```

## 2. Activate the Virtual Environment

### On macOS/Linux:
```bash
source venv/bin/activate
```

### On Windows (Command Prompt):
```cmd
venv\Scripts\activate
```

### On Windows (PowerShell):
```powershell
.\venv\Scripts\Activate.ps1
```

Once activated, your terminal prompt should show `(venv)`.

## 3. Install Required Packages

If you have a `requirements.txt` file, install dependencies using:

```bash
pip3 install -r requirements.txt
```

## 4. Create the SQLAlchemy database

If you're using SQLAlchemy as a Python SQL toolkit then run below commands in the python shell:

```
from app import app, db
with app.app_context():
    db.create_all()
```

## 4. Run the Flask Application

Make sure your application file (e.g., `app.py`) is correctly set up.

```
python3 app.py
```

## 5. Deactivate the Virtual Environment

When you're done with testing the project, deactivate the virtual environment using:

```bash
deactivate
```

You're now ready to develop and run your Flask application!
