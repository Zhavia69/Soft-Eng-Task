# Health Program Management System
A web-based application for healthcare providers to manage client enrollments in health programs (e.g., Malaria, HIV, Diabetes) with API integration.

## Features

- **Doctor Portal**:
  - Create health programs (predefined or custom)
  - Register clients with demographic data
  - Enroll clients in multiple health programs
  - View client profiles with enrollment history

- **API Integration**:
  - RESTful endpoint to fetch client data (`/api/client/<id>`)
  - JSON responses for system interoperability

## Technologies

- **Backend**: Python Flask
- **Frontend**: HTML5, CSS3, Jinja2 Templates
- **Database**: JSON (with SQLite-ready architecture)
- **Deployment**: Render/Fly.io (or Docker-compatible)

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/health-program-system.git
   cd health-program-system
Install dependencies:

bash
pip install flask python-dotenv
Run the application:

bash
python app.py
Access at: http://localhost:5000

API Documentation
Get Client Profile
GET /api/client/<client_id>
Response:

json
{
  "status": "success",
  "data": {
    "client_info": {
      "client_id": "123",
      "name": "John Doe",
      "age": 35,
      "gender": "Male"
    },
    "enrolled_programs": [
      {
        "name": "Diabetes",
        "description": "A metabolic disease..."
              }
    ]
  }
}
Project Structure
health-program-system/
├── app.py                # Flask application
├── data/                 # JSON database storage
│   ├── health_system.json
├── templates/            # HTML templates
│   ├── index.html
│   ├── register_client.html
│   └── ...
├── static/               # CSS/JS assets
├── README.md             # This file
└── requirements.txt      # Dependencies
Screenshots
Feature	Preview
Client Registration	Registration
Program Enrollment	Enrollment
Future Enhancements
Migrate to SQLite/PostgreSQL

Add authentication (JWT/OAuth)

Mobile-responsive design

Analytics dashboard

License
MIT License. See LICENSE for details.


### Key Enhancements:
1. **Visual Appeal**: Add screenshots in a folder
2. **Clear Navigation**: Structured sections with emoji icons
3. **API Focus**: Dedicated documentation for interoperability
4. **Deployment-Ready**: Includes setup instructions

### To Add:
1. Replace `yourusername` with your GitHub handle
2. Add actual screenshots (replace placeholder paths)
3. Update the `Future Enhancements` list with your roadmap

This README follows GitHub best practices with:
- **Badges-ready** (add build/coverage badges later)
- **Mobile-friendly** Markdown formatting
- **SEO-friendly** headers for discoverability
