# React Native Undefined is not an object (evaluating 'this.state.variable')
This repository demonstrates a common React Native error: 'undefined is not an object (evaluating 'this.state.variable')'. This occurs when accessing a state variable or prop before it's assigned a value, often due to asynchronous operations.

The `bug.js` file showcases the error, while `bugSolution.js` provides a solution using the useEffect hook and conditional rendering.

## How to reproduce the error
1. Clone this repository.
2. Run `npm install`.
3. Run `npx react-native run-android` or `npx react-native run-ios`.
4. Observe the error in the console.

## Solution
The solution involves using the useEffect hook to fetch data and only accessing state after it has been populated. Conditional rendering can prevent errors if data is still loading.