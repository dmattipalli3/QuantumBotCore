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
- Then choose firestore and functions for features you want to add in your directory
- Then for the codebase, it will give you the option to initialize or overwrite an existing codebase, we created one so do overwrite
- Then click yes for all additional files that firebase will provide for your project
- Click yes for installing all npm dependencies
- Then your firebase initialization will be complete
- After this, for the database create a collection, and then a subcollection, which will then store the respective data
- Create a folder in functions folder called api
- Then create a function in this folder, I created a function that would add message for simplicity
- After this make sure to go to the firebase console where your project is and change the plan from Spark to Blaze
- Go to Index.js and make sure to set the file for the function here
- Then enter command, firebase deploy --only functions
- You should get a message in the terminal saying the deployment was successful
- Then on the firebase console, you should be able to see your functions on the functions tab
- This is the endpoint being deployed to the cloud
- Download Postman and create an account
- Create a workspace for this specific project
- Get the link from the function in the firebase console which is the API endpoint
- Create a post request and paste the link here
- Go to headers, and add content type, and set the value to application/json
- Then go to body, and change to raw
- Enter the data for the add message function, or respective function
- If the data is valid, you should receive a success response in the output
- Now if you go the firestore database, you should the message ID there
