meteor-start-app
================

login with github

If you are new to meteor and just want to develop a start app for the meteor, than its a very good app which will explain you how to integerate a meteor app.

> Install meteroite:- 

  sudo npm install -g meteorite

  Meteorite is a packagemanager for Meteor. you can also use npm for handling packages, but Meteorite is a good choice because it supports the user submitted packages in the Atmosphere repo.

> Now start creating application:

  mrt create first_app

Now with this command your app will be created and when you will go inside the app you will find .js file first_app.js in which 
  // Shared code goes here
  
  if (Meteor.isClient) {
  
      // Client code
      
  }
  
  if (Meteor.isServer) {
  
    // Server code
    
  }
  
So to saperately define the client code and the server code we will remove these file by:
  cd chatapp
  rm chatapp.*
and create a saperate client and server by: 
  mkdir client server
So know your project will have:
  client/
  server/
  smart.json
  
Now write your client code inside the client folder and server code inside the server folder.

> For storing the database meteor use mongodb and to define the database we define it in a model.js we will create this file in an app and inside the model.js we will write:

  Messages = new Meteor.Collection('messages');
  

> For providing authentication to the app we use: 

  mrt add accounts-ui
  mrt add accounts-github


