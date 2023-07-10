# primaDiscuss_Realtime_chat
Installing the App Dependencies First, you need to have NodeJs installed on your machine. Second, you need to also have the React-CLI installed on your computer using the command below.

          npm install -g create-react-app
Next, create a new project with the name .

          npx create-react-app primadiscuss
Now, install these essential dependencies for our project using the command below.

          npm install react-router-dom

          npm install @material-ui/core

          npm install @material-ui/icons

          npm install firebase

          npm install moment react-moment

          npm install moment-timezone
Now that we're done with the installations, let's move on to building our solution.

Installing CometChat SDK

Head to CometChat Pro and create an account. From the dashboard, add a new app called "primadiscuss". Select this newly added app from the list. From the Quick Start, copy the APP_ID, REGION and AUTH_KEY, which will be used later. Also, copy the REST_API_KEY from the API & Auth Key tab. Navigate to the Users tab, and delete all the default users and groups leaving it clean (very important). Create a "app.config.js" in the src directory of the project. Enter your secret keys from CometChat and Firebase below on the next heading. Run the following command to install the CometChat SDK.

             npm install @cometchat-pro/chat@2.3.0 --save
The App Config File The setup below spells out the format for configuring the app.config.js files for this project.

const firebaseConfig = { apiKey: 'xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx',
                          authDomain: 'xxx-xxx-xxx-xxx-xxx-xxx-xxx',
                          databaseURL: 'xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx',
                          projectId: 'xxx-xxx-xxx', 
                          storageBucket: 'xxx-xxx-xxx-xxx-xxx', 
                          messagingSenderId: 'xxx-xxx-xxx', 
                          appId: 'xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx', 
                          measurementId: 'xxx-xxx-xxx', },

const cometChat = { APP_ID: 'xxx-xxx-xxx',
                    AUTH_KEY: 'xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx',
                    REST_KEY: 'xxx-xxx-xxx-xxx-xxx-xxx-xxx-xxx',
                    APP_REGION: 'xx', }

export { firebaseConfig, cometChat }
