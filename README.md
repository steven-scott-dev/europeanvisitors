[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Build Status](https://img.shields.io/github/actions/workflow/status/steven-scott-dev/europeanvisitors/ci.yml)](https://github.com/steven-scott-dev/europeanvisitors/actions)
[![Coverage Status](https://img.shields.io/codecov/c/github/steven-scott-dev/europeanvisitors)](https://codecov.io/gh/steven-scott-dev/europeanvisitors)

# European Visitors

European Visitors is a full-stack travel-planning app that helps users explore Europe with curated destination guides, interactive maps, and itinerary management. Built with a Django REST API backend and a React/Redux frontend, it features user authentication, dynamic content fetching, responsive design, and seamless UX across devices.

---

## Table of Contents

- [Demo](#demo)  
- [Tech Used](#tech-used)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Environment Variables](#environment-variables)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Demo

> **Note:** On the free Heroku plan the backend sleeps after inactivity, so initial load may take a few seconds.

- **Frontend live:** https://european-visitors-frontend.herokuapp.com/  
- **API live (Swagger):** https://european-visitors-backend.herokuapp.com/swagger/  

---

## Tech Used

- **Frontend:** React, Redux  
- **Backend:** Django, Django REST Framework  
- **Languages & Tools:** JavaScript (ES6+), Python, HTML5, CSS3  
- **Database:** PostgreSQL (via Heroku)  

---

## Installation

1. **Clone the repo**  
   ```bash
   git clone https://github.com/steven-scott-dev/europeanvisitors.git
   cd europeanvisitors
Backend setup

bash
Copy code
cd backend
python -m venv env
# macOS/Linux
source env/bin/activate
# Windows PowerShell
.\env\Scripts\Activate.ps1

pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate

# (Optional) Load dummy data for testing:
python manage.py loaddata fixtures/dummy-data.json

python manage.py runserver
# Backend serves at http://127.0.0.1:8000/
Frontend setup

bash
Copy code
cd ../frontend
npm install
npm start
# Frontend serves at http://localhost:3000/
Usage
User flow:

Sign up or log in

Browse curated guides

Add destinations to your itinerary

View interactive map with saved stops

Admin access:

bash
Copy code
cd backend
python manage.py createsuperuser
Environment Variables
Create a .env file in the backend/ folder with at least:

env
Copy code
DJANGO_SECRET_KEY=your_secret_here
DATABASE_URL=postgres://username:password@host:port/dbname
Add any other API tokens or keys as needed.

Contributing
See CONTRIBUTING.md for:

Fork & branch workflow

Code style & linting rules

Pull request guidelines

We welcome improvements, bug fixes, and new features—just follow the guidelines!

License
This project is licensed under the MIT License. See the LICENSE file for details.