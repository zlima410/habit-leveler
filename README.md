# Habit Tracker App

A cross-platform habit-tracking app built with React Native (Expo), Django (REST API backend), and Firebase. This app includes features for tracking daily, weekly, monthly, and annual habits, with a gamified leveling system that rewards users with more XP for completing higher-frequency tasks. Secure authentication is provided via Firebase OAuth.

## Features

- **Habit Tracking**: Organize habits based on frequency (daily, weekly, monthly, annual).
- **Gamified Leveling System**: Gain experience points (XP) and level up based on habit completion. Higher-frequency tasks yield more XP.
- **Secure Authentication**: Log in via Google OAuth using Firebase Authentication.
- **Backend API**: Django REST API for data handling and user management.
- **Real-time Data**: Track progress and sync across devices using Firebase Firestore.

## Tech Stack

- **Frontend**: React Native with Expo
- **Backend**: Django with Django REST Framework
- **Database**: Firebase Firestore for real-time data
- **Authentication**: Firebase Authentication with Google OAuth

## Getting Started

### Prerequisites

- **Node.js** (v14 or higher)
- **Python** (v3.8 or higher)
- **Expo CLI**
- **Firebase Account**

### Installation

1. **Clone the Repository**
   ```bash
   git clone <your-repository-url>
   cd habit-tracker-app```

2. **Set Up Frontend (React Native)**
   ```cd frontend
   npm install```

3. **Set Up Backend (Django)**
   ```cd ../backend
   pip install -r requirements.txt```

Project Structure

```habit-tracker-app/
├── frontend/                 # React Native frontend
│   ├── src/                  # React Native source files
│   ├── .env                  # Environment variables for Firebase
│   └── app.config.js         # Expo configuration file
└── backend/                  # Django backend
    ├── habits/               # Django app for habits feature
    ├── .env                  # Environment variables for Django
    └── settings.py           # Django settings file```

Security and Sensitive Data

    Environment Variables: Sensitive data is stored in .env files, which are not tracked in Git. Ensure .env files are listed in .gitignore.
    Firebase Credentials: Firebase Admin credentials are stored in a secure location and loaded from environment variables in Django.
