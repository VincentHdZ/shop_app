# shop_app

A new Flutter project.

## Getting Started

This project need to use Firebase. Follow the next steps :

///PREPARE BACKEND FOR CRUD///

- Go to https://firebase.google.com/ and connect with yout google account
- Click on "Go to console" in the top right corner
- Click on "create a project" and follow steps
- You don't need "Google Analytics"
- In the Project Overview, on the left click on " Build=>Realtime Database"
- Click on "Create database" and follow steps
- You should have a link like this => https://mydatabase.firebaseio.com/
- Take a search in the flutter project on "TODO:firebaseio.com"
- In the final variable "url" replace the "https://mydatabase.firebaseio.com/" with yours

///PREPARE BACKEND FOR AUTHENTICATION///

- Go back to your realtime Database and click on "Rules"
- Copy and path the following rules : 
{
  "rules": {
    ".read": "auth != null",
    ".write": "auth != null",
  }
}
- Click on "publish"
- In the Project Overview, on the left, go to "Build=>Authentication"
- Click on "set up sign-in method"
- Click on "Email/Password" and click on the first "enable" button
- In the top left corner click on settings => project settings
- Copy the "Web API Key"
- Take a search in the flutter project on "//TODO:https://www.googleapis.com/identitytoolkit/v3/relyingparty"
- In the final url replace key="web api value" with yours

