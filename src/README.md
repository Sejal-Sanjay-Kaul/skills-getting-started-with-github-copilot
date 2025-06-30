# Mergington High School Activities API

A super simple FastAPI application that allows students to view and sign up for extracurricular activities.

## Features

- View all available extracurricular activities
- Sign up for activities
- Simple web interface for students

## Getting Started

1. Install the dependencies:

   ```bash
   pip install fastapi uvicorn
   ```

2. Run the application (recommended):

   ```bash
   uvicorn app:app --reload
   ```
   
   Or, if you prefer:
   ```bash
   python app.py
   ```

3. Open your browser and go to:
   - Web UI: http://localhost:8000/static/index.html
   - API documentation: http://localhost:8000/docs
   - Alternative documentation: http://localhost:8000/redoc

## API Endpoints

| Method | Endpoint                                                          | Description                                                         |
| ------ | ----------------------------------------------------------------- | ------------------------------------------------------------------- |
| GET    | `/activities`                                                     | Get all activities with their details and current participant count |
| POST   | `/activities/{activity_name}/signup?email=student@mergington.edu` | Sign up for an activity                                             |

## Data Model

The application uses a simple data model with meaningful identifiers:

1. **Activities** - Uses activity name as identifier:

   - Description
   - Schedule
   - Maximum number of participants allowed
   - List of student emails who are signed up

2. **Students** - Uses email as identifier:
   - Name
   - Grade level

All data is stored in memory, which means data will be reset when the server restarts.

## Features to Try

- Sign up for an activity using your email.
- View available activities and their schedules.
- See the number of participants in each activity.
- Enjoy a modern, responsive web interface with improved colors and layout.

## How to Contribute

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## Credits

Designed, developed, and maintained by Sejal. 
GitHub: [Sejal](https://github.com/)
