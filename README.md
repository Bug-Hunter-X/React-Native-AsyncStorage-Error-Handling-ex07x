# React Native AsyncStorage Error Handling

This repository demonstrates a common error in React Native applications when using AsyncStorage: the lack of proper error handling. AsyncStorage operations (getItem and setItem) can throw exceptions, leading to app crashes.  This example shows the flawed code and the corrected version with robust error handling.

## Bug

The `bug.js` file contains code that attempts to use AsyncStorage without a try...catch block.  This means any errors thrown by AsyncStorage will cause the application to terminate unexpectedly.

## Solution

The `bugSolution.js` file demonstrates the correct way to handle potential errors using try...catch blocks and logging any issues to the console. This prevents unexpected crashes and provides more robust error handling.

## How to Run

1. Clone this repository.
2. Navigate to the project directory using your terminal.
3. Run `npm install` to install the required dependencies.
4. Run `npx react-native run-android` (or `npx react-native run-ios`) to start the app on your emulator or device. Observe the behavior of both the buggy and corrected version of the code.