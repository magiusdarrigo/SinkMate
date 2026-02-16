# SinkMate

Protect you and others without thinking about it.

**Hackathon Winner** - [View on Devpost](https://devpost.com/software/sinkmate)

## About

SinkMate is a web-based music streaming platform that lets users discover and stream over 20,000 songs with a single click. Built during a hackathon, it focuses on delivering a seamless, intuitive listening experience.

## Tech Stack

- **Frontend:** HTML5, CSS3, JavaScript
- **Backend:** Node.js, Firebase Cloud Functions, Express.js
- **Database:** Firebase Realtime Database, Cloud Firestore
- **Auth:** Firebase Authentication
- **Storage:** Firebase Cloud Storage
- **Hosting:** Firebase Hosting

## Project Structure

```
SinkMate/
├── public/              # Static web assets
│   ├── index.html       # Default hosting page
│   ├── landing.html     # Main landing page
│   ├── discover.html    # Music discovery page
│   ├── 404.html         # Custom error page
│   ├── styles.css       # Global styles
│   └── landing.css      # Landing page styles
├── functions/           # Firebase Cloud Functions
│   ├── index.js         # Functions entry point
│   └── package.json     # Backend dependencies
├── images/              # Visual assets (logo, icons, covers)
├── firebase.json        # Firebase configuration
├── firestore.rules      # Firestore security rules
├── database.rules.json  # Realtime Database rules
└── storage.rules        # Cloud Storage rules
```

## Getting Started

### Prerequisites

- Node.js (v14+)
- npm
- [Firebase CLI](https://firebase.google.com/docs/cli)
- A Firebase account

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/SinkMate.git
cd SinkMate

# Install Cloud Functions dependencies
npm install --prefix functions

# Install Firebase CLI (if not already installed)
npm install -g firebase-tools

# Log in to Firebase
firebase login
```

### Running Locally

```bash
# Start the Firebase emulator
firebase emulators:start

# Or run Cloud Functions only
npm --prefix functions run serve
```

### Deployment

```bash
# Deploy everything (hosting + functions)
firebase deploy

# Deploy only Cloud Functions
npm --prefix functions run deploy

# View function logs
npm --prefix functions run logs
```

## Features

- **Music Discovery** - Browse and explore a catalog of songs
- **One-Click Streaming** - Start listening instantly
- **User Accounts** - Sign up and manage your profile via Firebase Auth
- **Real-Time Data** - Live updates powered by Firebase Realtime Database
- **Responsive Design** - Works across desktop and mobile browsers

## License

This project is open source.
