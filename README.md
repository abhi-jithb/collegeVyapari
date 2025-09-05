# CollegeVyapari

A React Native mobile app for college students to connect, collaborate, and help each other with academic tasks, deliveries, and campus services.

## What is CollegeVyapari?

CollegeVyapari is a peer-to-peer platform designed specifically for college students. Whether you need help with assignments, want someone to deliver food from the mess, or looking for study partners - this app connects you with fellow students who can help!

Key Features:
- Academic Help - Get assistance with assignments and projects
- Campus Delivery - Food delivery, book sharing, and more
- Task Management - Post and manage your requests easily
- Budget-friendly - Set your own prices for services
- Rating System - Build trust through community ratings

## Prerequisites

Before you start, make sure you have these installed on your computer:

### For Windows Users:
1. **Node.js** (v18 or higher) - https://nodejs.org/
2. **Android Studio** - https://developer.android.com/studio
3. **Git** - https://git-scm.com/

### For Mac Users:
1. **Node.js** (v18 or higher) - https://nodejs.org/
2. **Xcode** (for iOS development) - Install from App Store
3. **Android Studio** (for Android development) - https://developer.android.com/studio
4. **Git** - https://git-scm.com/

**Detailed Setup Guide**: Follow the official React Native Environment Setup guide for your operating system:
https://reactnative.dev/docs/set-up-your-environment

## Installation & Setup

### Step 1: Clone the Repository
git clone https://github.com/rsreehari/collegeVyapari.git
cd collegeVyapari

text

### Step 2: Install Dependencies
npm install

text

### Step 3: Android Setup (Required for Android development)

1. **Configure Android SDK path** in `android/local.properties`:
sdk.dir=C:\Users\YourUsername\AppData\Local\Android\Sdk

text

2. **Start an Android emulator** or connect your physical device with USB debugging enabled

### Step 4: iOS Setup (Mac only)
cd ios
bundle install
bundle exec pod install
cd ..

text

## Running the App

### Method 1: Using npm (Recommended for beginners)

1. **Start the Metro bundler** (keep this running):
npm start

text

2. **Open a new terminal** and run the app:

**For Android:**
npm run android

text

**For iOS (Mac only):**
npm run ios

text

### Method 2: Using React Native CLI

1. **Start Metro bundler**:
npx react-native start

text

2. **Run the app** (in a new terminal):
For Android
npx react-native run-android

For iOS (Mac only)
npx react-native run-ios

text

## Development Workflow

### Making Changes
1. Open the project in **VS Code** or your preferred editor
2. Edit files in the `src/` directory
3. Save your changes - the app will **automatically reload** thanks to Fast Refresh!

### Manual Reload (if needed)
- **Android**: Press `R` twice or `Ctrl+M` (Windows) / `Cmd+M` (Mac) to open Dev Menu
- **iOS**: Press `R` in the iOS Simulator

### Project Structure
collegeVyapari/
├── src/
│ ├── components/ # Reusable UI components
│ ├── screens/ # App screens (Home, Profile, Tasks, etc.)
│ ├── navigation/ # Navigation setup
│ └── utils/ # Helper functions
├── android/ # Android-specific code
├── ios/ # iOS-specific code (Mac only)
└── package.json # Dependencies and scripts

text

## Common Issues & Solutions

### Port Already in Use
Kill the process using port 8081
fuser -k 8081/tcp

Or on Windows
netstat -ano | findstr :8081
taskkill /PID <PID_NUMBER> /F

text

### Metro Bundler Won't Start
Clear Metro cache
npx react-native start --reset-cache

text

### Android Emulator Issues
Restart ADB
adb kill-server
adb start-server

Check connected devices
adb devices

text

### Build Errors
Clean build
cd android
./gradlew clean
cd ..

Rebuild
npm run android

text

### Node Modules Issues
Delete node_modules and reinstall
rm -rf node_modules
npm install

text

### Git Issues
Fix common Git commit message errors
git commit -m "your commit message" # Note: no space between - and m

Push changes
git add .
git commit -m "your message"
git push origin your-branch-name

text

### React Native CLI vs npm scripts
These are equivalent:
npm run android # Same as: npx react-native run-android
npm run ios # Same as: npx react-native run-ios
npm start # Same as: npx react-native start

text

## Testing on Physical Device

### Android Device:
1. Enable **Developer Options** in Settings
2. Turn on **USB Debugging**
3. Connect device via USB
4. Run `adb devices` to verify connection
5. Run `npm run android`

### iOS Device (Mac only):
1. Connect device via USB
2. Open Xcode and sign the app with your Apple ID
3. Trust the developer certificate on your device
4. Run `npm run ios`

## Quick Start Commands (Copy & Paste)

### First Time Setup:
git clone https://github.com/rsreehari/collegeVyapari.git
cd collegeVyapari
npm install

text

### Daily Development:
Terminal 1 - Start Metro
npm start

Terminal 2 - Run app
npm run android

OR
npm run ios

text

### When Things Break:
Clear everything and restart
rm -rf node_modules
npm install
npx react-native start --reset-cache

text

### Git Workflow:
git add .
git commit -m "describe your changes"
git push origin main

text

## Learning Resources

### React Native Basics:
- **Official Docs**: https://reactnative.dev/docs/getting-started
- **Tutorial**: https://reactnative.dev/docs/tutorial
- **Components**: https://reactnative.dev/docs/components-and-apis

### JavaScript & React:
- **JavaScript Guide**: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide
- **React Docs**: https://react.dev/
- **React Hooks**: https://react.dev/reference/react

### Debugging:
- **React Native Debugger**: https://github.com/jhen0409/react-native-debugger
- **Flipper**: https://fbflipper.com/
- **Console Logs**: Use `console.log()` in your code to debug

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Support

If you encounter any issues or have questions:

1. Check the **Common Issues** section above
2. Visit the [React Native Troubleshooting Guide](https://reactnative.dev/docs/troubleshooting)
3. Create an issue in this repository
4. Join the [React Native Community](https://reactnative.dev/help)

## Useful Tips for Beginners

### Development Environment:
- Use **VS Code** with React Native extensions
- Keep **Android Studio** open for emulator management
- Use **Git Bash** or **PowerShell** for Windows

### Code Organization:
- Keep components small and reusable
- Use meaningful variable and function names
- Comment your code for future reference

### Testing:
- Test on both Android and iOS if possible
- Use physical devices for better performance testing
- Test on different screen sizes

### Performance:
- Use `console.log()` sparingly in production
- Optimize images and assets
- Use FlatList for long lists instead of ScrollView

## Common File Locations

Important files you'll work with:
├── App.tsx # Main app entry point
├── src/screens/ # Your app screens
├── src/components/ # Reusable components
├── android/local.properties # Android SDK path
├── package.json # Dependencies
└── README.md # This file

text

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

**Happy Coding!** This app is built by students, for students. Let's make college life easier together.

**Need help?** Don't hesitate to ask questions or create issues in this repository. We're all learning together!
