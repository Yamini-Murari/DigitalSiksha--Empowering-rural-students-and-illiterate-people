# DigitalSiksha--Empowering-rural-students-and-illiterate-people

DigitalSiksha 📱🎓

Digital Empowerment for All

DigitalSiksha is a React Native mobile application designed to promote digital literacy. It provides video lessons, quizzes, and progress tracking in multiple Indian languages to help users master basic computer skills, internet usage, and digital safety.

🌟 Features

Trilingual Support: Full interface and content support for English, Hindi, and Telugu.

Video Learning Paths: Curated video lessons on Computer Basics, Internet, Banking, Government Services, and Wellness.

Interactive Quizzes: Test your knowledge after every lesson with instant feedback.

Gamification: Earn badges (Beginner, Learner, Achiever, Master) as you progress.

Text-to-Speech: Built-in voice guide to assist users with navigation and accessibility.

Offline Mode (Simulated): Download videos to watch later without an internet connection.

Certificate Generation: View and download a completion certificate upon finishing courses.

User Profiles: Track progress and manage personal details.

🛠️ Tech Stack

Framework: React Native (via Expo)

Video Playback: expo-av

Text-to-Speech: expo-speech

UI Styling: expo-linear-gradient, standard React Native StyleSheet

Storage: @react-native-async-storage/async-storage (for persisting user progress and settings)

🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

Prerequisites

Node.js (LTS version recommended)

Expo Go app installed on your Android/iOS device.

Installation

Clone the repository:

git clone [https://github.com/YOUR_USERNAME/digital-siksha-app.git](https://github.com/YOUR_USERNAME/digital-siksha-app.git)
cd digital-siksha-app


Install dependencies:

npm install


Install required Expo libraries:
This project relies on specific native libraries. Run this command to ensure they are installed correctly:

npx expo install expo-av expo-speech expo-linear-gradient @react-native-async-storage/async-storage


⚙️ Configuration Note (Important)

This project uses a Single File Entry (Classic) structure, not the modern Expo Router file-based routing.

If you are setting this up in a new environment, ensure your package.json file points to App.jsx as the main entry point:

"main": "App.jsx"


(If "main" is set to "expo-router/entry", the app will not load correctly).

📱 Running the App

Start the development server:

npx expo start


On your phone:

Open the Expo Go app.

Scan the QR code displayed in your terminal.

On an Emulator:

Press a for Android Emulator.

Press i for iOS Simulator.

📂 Project Structure

DigitalSikshaApp/

├── assets/web             # Images, fonts, and local videos

│   └── videos/          # Store local MP4 files here

├── App.jsx              # MAIN APP LOGIC (All navigation and screens)

├── app.json             # Expo configuration

├── package.json         # Dependencies and scripts

└── README.md            # Project documentation


🧩 Adding Custom Videos

To replace the placeholder videos with your own:

Place your .mp4 file in the assets/videos/ folder.

In App.jsx, locate the videoData object.

Change the URL to a require statement:

url: {
    en: require('./assets/videos/my-video.mp4'),
    // ...
}


Restart the server with npx expo start --clear to load the new assets.

📄 License

This project is open-source and available for educational purposes.

Built with ❤️ for Digital Literacy
