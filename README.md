# Health-tracker
 A Python-based command-line application for tracking and managing personal health metrics including steps, sleep, calories, water intake, and heart rate.
Features
•	User Management: Secure registration and login system
•	Health Metrics Logging: Track daily health data including: 
o	Steps walked
o	Sleep duration
o	Calories consumed
o	Water intake
o	Average heart rate
•	Data Management: View, update, and delete health logs
•	Analytics: Automatic activity classification and health summaries
•	Persistent Storage: JSON-based data storage for user profiles and logs
Requirements
•	Python 3.6 or higher
•	No external dependencies required (uses standard library only)
Installation
1.	Clone or download the repository
2.	Navigate to the project directory
3.	Run the application:
bash
python health_dashboard.py
Usage
First Time Users
1.	Select option 1 to Register
2.	Create a username and password
3.	Enter your profile information (name, age, height, weight)
4.	Login with your credentials
Daily Usage
1.	Login with your credentials
2.	Select option 1 to log today's health metrics
3.	Enter your daily measurements
4.	View summaries and track progress over time
Main Menu Options
•	Register: Create a new user account
•	Login: Access your personal dashboard
•	Exit: Save data and close application
User Dashboard Options
1.	Log today's health metrics: Add new daily health data
2.	View all logs: Display all recorded health entries
3.	Update a log: Modify existing health records
4.	Delete a log: Remove specific health entries
5.	View summary & activity classification: See aggregated statistics and activity level
6.	Logout: Return to main menu
Activity Classification
The system automatically classifies your activity level based on average daily steps:
•	Sedentary: < 5,000 steps
•	Lightly Active: 5,000 - 7,999 steps
•	Active: 8,000 - 9,999 steps
•	Very Active: ≥ 10,000 steps
Health Recommendations
The application provides personalized suggestions:
•	Sleep recommendation if average < 7 hours
•	Water intake reminder if average < 2 liters
Data Storage
All user data is stored locally in health_data.json in the following structure:
json
{
  "username": {
    "password": "user_password",
    "profile": {
      "name": "Full Name",
      "age": 25,
      "height": 1.75,
      "weight": 70.0
    },
    "logs": [
      {
        "date": "2025-01-15",
        "steps": 8500,
        "sleep_hours": 7.5,
        "calories": 2200,
        "water_liters": 2.5,
        "avg_heart_rate": 72
      }
    ]
  }
}






