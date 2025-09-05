# CollegeVyapari

A React Native mobile app for college students to connect, collaborate, and help each other.

## Project Setup

1. Clone the repository:

```

git clone https://github.com/rsreehari/collegeVyapari.git

cd collegeVyapari

```

2. Install dependencies:

```

npm install

```

3. Start Metro bundler:

```

npx react-native start

```

4. Run on Android:

```

npx react-native run-android

```

## Notes

- Make sure your Android SDK path is correct in `android/local.properties`.

- If you see port errors, kill the process using `fuser -k 8081/tcp`.

- For Windows users, use `netstat -ano | findstr :8081` then `taskkill /PID <PID> /F`.

This is a new [**React Native**](https://reactnative.dev) project for college students,

# Getting Started

> **Note**: Make sure you have completed the [Set Up Your Environment](https://reactnative

## Prerequisites

Before starting, ensure you have:

- **Node.js** (v18 or higher) - [Download](https://nodejs.org/)

- **Android Studio** with Android SDK - [Download](https://developer.android.com/studio)

- **Git** for version control - [Download](https://git-scm.com/)

- **VS Code** or your preferred editor

## Step 1: Start Metro

First, you will need to run **Metro**, the JavaScript build tool for React Native.

To start the Metro dev server, run the following command from the root of your React Native

```

# Using npm

npm start

# OR using Yarn

yarn start

```

## Step 2: Build and run your app

With Metro running, open a new terminal window/pane from the root of your React Native 

### Android

```

# Using npm

npm run android

# OR using Yarn

yarn android

```

### iOS

For iOS, remember to install CocoaPods dependencies (this only needs to be run on first command)

```

bundle install

bundle exec pod install

```

```

# Using npm

npm run ios

# OR using Yarn

yarn ios

```

## Step 3: Configure Android SDK

Configure your Android SDK path in `android/local.properties`:

```

sdk.dir=C:\\Users\\YourUsername\\AppData\\Local\\Android\\Sdk

```

## Step 4: Modify your app

Now that you have successfully run the app, let's make changes!
Open files in `src/screens/` or `src/components/` and make changes. The app will automatic

### Manual Reload

- **Android**: Press <kbd>R</kbd> key twice or <kbd>Ctrl</kbd> + <kbd>M</kbd> for Dev Men

- **iOS**: Press <kbd>R</kbd> in iOS Simulator

## Testing on Physical Device

### Android Device

```

# Enable Developer Options and USB Debugging on your phone

# Connect via USB, then verify:

adb devices

# Run the app:

npm run android

```

### iOS Device (Mac only)

```

# Connect device, sign in Xcode, then:

npm run ios

```

# Troubleshooting

## Common Issues

### Port Already in Use

```

# Kill process on port 8081

fuser -k 8081/tcp

# Windows:

netstat -ano | findstr :8081

taskkill /PID <PID_NUMBER> /F

```

### Metro Bundler Issues

```

# Clear cache

npx react-native start --reset-cache

```

### Android Problems

```

# Restart ADB

adb kill-server

adb start-server

adb devices

```

### Build Errors

```

# Clean build

cd android

./gradlew cleancd ..

npm run android

```

### Node Modules Issues

```

# Reinstall dependencies

rm -rf node_modules

npm install

```

### Git Issues

```

# Correct commit syntax (no space between - and m)

git commit -m "your message"

```

## Quick Commands

```

# Daily workflow

npm start # Terminal 1

npm run android # Terminal 2

# When broken

rm -rf node_modules && npm install

npx react-native start --reset-cache

# Git workflow

git add .

git commit -m "describe changes"

git push origin main

```

# Learn More

- [React Native Website](https://reactnative.dev)

- [Getting Started](https://reactnative.dev/docs/environment-setup)

- [Components Reference](https://reactnative.dev/docs/components-and-apis)

- [Troubleshooting Guide](https://reactnative.dev/docs/troubleshooting)

## CollegeVyapari Features

- **Task Management** - Post and manage academic tasks

- **Campus Delivery** - Food delivery and item sharing

- **Rating System** - Community trust building

- **Category Filters** - Academic, Delivery, Events, etc.

---

**Happy Coding!** Built by students, for students.

```

Copy everything between the `````markdown` and ```
