# Firebase Setup Guide

This guide explains how to set up Firebase, Node.js, and npm for your project.

## Steps to Follow

1. **Download and Install Node.js (LTS Version)**  
   Visit the official Node.js website: [https://nodejs.org/en/](https://nodejs.org/en/).  
   Download the LTS version and run the installer. During the installation:  
   - Once completed, a CMD window might pop up; you can close it if you dont need to install Visual Studio Tools and Python.

2. **Change PowerShell Execution Policy**  
   Open PowerShell as Administrator and follow these steps:  
   - Check the current execution policy:  
     `Get-ExecutionPolicy`  
     If the output is `Restricted`, proceed with the next steps. Otherwise, skip to step 3.  
   - Change the execution policy:  
     `Set-ExecutionPolicy RemoteSigned`  
     Type `Y` (Yes) to confirm.  
   - Verify npm installation:  
     `npm -v`  
     If installed correctly, it will show the version (e.g., `10.9.0`).

3. **Install Firebase CLI Tools**  
   Use npm to install Firebase CLI globally:  
   `npm install -g firebase-tools`

4. **Check Firebase CLI Installation**  
   Verify that Firebase CLI is installed correctly:  
   `firebase --version`

5. **Log in to Firebase**  
   Authenticate with your Firebase account:  
   `firebase login`

6. **Initialize Firebase (if needed)**  
   For a new project:  
   `firebase init`  
   If the project is cloned, this step is **not necessary**.

7. **Preview or Deploy the Project**  
   - To preview your project locally:  
     `firebase serve`  
   - To deploy your project to Firebase Hosting:  
     `firebase deploy`
