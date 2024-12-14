# Expo Camera takePictureAsync Error

This repository demonstrates a common error encountered when using Expo's Camera API: attempting to use `takePictureAsync` before the camera is fully initialized.  The provided solution addresses this issue by ensuring the `takePicture` function is only called after the camera is ready.

## Problem

Calling `takePictureAsync` before the camera has finished initializing leads to errors. The code in `bug.js` showcases this incorrect usage resulting in a failure to capture images.

## Solution

The `bugSolution.js` file offers a corrected approach. The solution includes waiting for the `onCameraReady` event emitted by the Expo Camera component before allowing the user to take a picture.  This guarantees that the camera is prepared and ready to capture images, preventing the error.

## How to Run

1. Clone this repository.
2. `npm install`
3. Run the app using Expo Go or a similar Expo client.