# Silent Crash in React Native Due to Unhandled Promise Rejection

This repository demonstrates a common yet easily missed bug in React Native applications: silent crashes due to unhandled promise rejections within the `useEffect` hook.  The bug occurs when a network request fails, and the resulting error isn't properly caught and handled.  The application crashes without providing any user-friendly error messages.

The provided solution showcases how to correctly handle these rejections to prevent silent crashes and provide better user feedback.

## Steps to Reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Run `npm install` to install dependencies.
4. Run the application using a React Native emulator or device.
5. Observe that the app crashes silently if the network request fails (e.g., due to a lack of internet connection).