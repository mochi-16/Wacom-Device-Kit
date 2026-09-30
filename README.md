# Wacom STU-430 Setup and Verification Guide

This folder contains the required Wacom SigCaptX service installer and sample HTML test pages for the STU-430 signature pad.

## 1) Install the SigCaptX service

IMPORTANT:

- Unplug the Wacom STU device before installing the service.
- Run the installer file located in this folder:
  - `Wacom-STU-SigCaptX-x64-2.18.0.exe`
- Complete the installation process.
- Restart the computer after the installation finishes.
- After the computer restarts, plug the Wacom STU device back in.

This is required before the device can be detected and used correctly.

## 2) Verify the SigCaptX service is running

To confirm that the service is properly running:

1. Open the file in the `PortCheck` folder:
   - `PortCheck/PortCheck.html`
2. Open it in a browser.
3. In the page, set the service port to:
   - `9000`
4. Click the "Check Service" button.
5. Confirm that the connection to the SigCaptX service is established.

You should see a successful service status in the output area. If the page reports the service is not connected, the service is not ready and the device should not be tested yet.

## 3) Test the STU device

Only after the SigCaptX service has already been confirmed to be functioning should you test the actual device.

1. Open the sample page in the `demobuttons` folder:
   - `demobuttons/demobuttons.html`
2. Open it in a browser.
3. Check the page functions and verify that the signature pad is working as expected.

This sample page is intended to validate the device functionality after the service is confirmed to be running.

## 4) Troubleshooting

If you encounter any error or issue that is not described in this README, contact technical support for assistance.

## Summary

Use this sequence:

1. Unplug the STU device.
2. Install `Wacom-STU-SigCaptX-x64-2.18.0.exe`.
3. Restart the computer.
4. Plug the STU device back in.
5. Open `PortCheck/PortCheck.html` and verify port `9000` is connected.
6. Open `demobuttons/demobuttons.html` and test the device functionality.
7. If an issue remains, contact technical support.
