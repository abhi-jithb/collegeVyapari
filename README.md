CollegeVyapari
CollegeVyapari is a campus marketplace app built with React Native.
It helps students buy, sell, or exchange items within their college community.
Getting Started
Follow these steps to run the project on your system.
1. Install dependencies
Copy code
Sh
npm install
2. Start the Metro bundler
Metro is the JavaScript build tool for React Native.
Copy code
Sh
npx react-native start
3. Run the app on Android
Copy code
Sh
npx react-native run-android
4. Run the app on iOS (Mac only)
First install CocoaPods (only the first time or after updating dependencies):
Copy code
Sh
bundle install
bundle exec pod install
Then run the app:
Copy code
Sh
npx react-native run-ios
Notes
Make sure your Android SDK path is set correctly in android/local.properties.
If you get a port already in use error:
Copy code
Sh
fuser -k 8081/tcp
You can also run the app directly using Android Studio or Xcode.
Modify the App
Open App.tsx in your editor.
Save changes and the app will auto-refresh with Fast Refresh.
Reloading manually
Android → press R twice or open Dev Menu (Ctrl+M / Cmd+M).
iOS → press R in the iOS Simulator.
Tech Stack
React Native
TypeScript
Metro Bundler
Android/iOS Emulator
Troubleshooting
If you face issues, check the React Native Troubleshooting guide.
Learn More
React Native Docs
Learn the Basics
Integration with existing apps
React Native Blog
Congratulations
You’ve set up and run CollegeVyapari successfully.
