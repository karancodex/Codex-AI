# CodeX AI - React Native Chatbot with Gemini API

A cross-platform mobile chatbot application powered by Google's Gemini AI, built with React Native. Features dark/light mode, chat history, and markdown support.

## Features

- 💬 Chat with Google's Gemini AI
- 🌙 Dark/Light mode toggle
- 📚 Chat history management
- ✨ Markdown support for responses
- 📱 Cross-platform (iOS & Android)

## Prerequisites

- Node.js (v16 or newer)
- npm or yarn
- React Native CLI
- Android Studio (for Android)
- Xcode (for iOS)
- Google Gemini API key

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/karancodex/Codex-AI.git
   cd Codex-AI
Install dependencies

bash
npm install
# or
yarn install
Set up environment variables
Create a .env file in the root directory:

env
CODEXAI_API_KEY=your_gemini_api_key_here
Link vector icons

bash
npx react-native link react-native-vector-icons
Gemini API Integration
Get your API key:

Go to Google AI Studio

Create an API key for the Gemini Pro model

Configure the API:
The app uses the Gemini Pro model with this endpoint:

javascript
`https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=${Config.CODEXAI_API_KEY}`
Request format:
The app sends requests in this format:

javascript
{
  contents: [{
    parts: [{ text: inputText }],
  }],
}
Running the App
Android
bash
npx react-native run-android
iOS
bash
cd ios && pod install && cd ..
npx react-native run-ios
Project Structure
/src
  /components      # Reusable components
  /constants       # App constants
  /contexts        # Context providers
  /hooks           # Custom hooks
  /screens         # Main screens
  /services        # API services
  /styles          # Global styles
  /types           # TypeScript types
  /utils           # Utility functions
Configuration
Edit app.config.js to:

Change app name

Configure splash screen

Set up deep linking

Troubleshooting
Icons not showing?

bash
npx react-native link react-native-vector-icons
# For iOS:
cd ios && pod install && cd ..
Environment variables not working?

Ensure you have react-native-config properly installed

For Android, add to android/app/build.gradle:

gradle
apply from: project(':react-native-config').projectDir.getPath() + "/dotenv.gradle"
Contributing
Fork the project

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

License
Distributed under the MIT License. See LICENSE for more information.

Contact
Your Name - Karan Maurya 

email- reachtokarankumar@gmail.com

Project Link: https://github.com/karancodex/Codex-AI.git

