# QuantumBotCore
Backend Project for Radical AI
- First install Node js and VS Code
- VS Code has a built in terminal, so use this for the remainder of the project
- Check to see if Node js had a successful configuration by entering command node --version in terminal
- Then you can do command npm install -g firebase-tools, permissions on my laptop were denying this command
- So I had to use sudo npm install -g firebase-tools
- Enter command firebase login, will prompt you to login
- Go to console.firebase.google.com
- Create a new project
- Create a firebase database for the project you just created, and make sure to put it in TESTING MODE
- After this enter the command firebase init, which will initialize your project for firebase
- Then choose firestore and functions for feautures you want to add in your directory
- Then for the codebase, it will give you the option to initialize or overwrite an existing codebase, we created one so do overwrite
- Then click yes for all additional files that firebase will provide for your project
- Click yes for installing all npm dependencies
- Then your firebase initialization will be complete
