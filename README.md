# Authentication_Mechanism_Using_Express-Nodejs
I have created an authentication mechanism to learn how JWT authentication mechanism and refresh tokens work. The tech stack used is Express, Nodejs and in memory database.
# Demo
Register new user
![Register new user](https://github.com/Lucifer7355/Authentication_Mechanism_Using_Express-Nodejs/blob/main/demonstration_pictures/Screenshot%20(262).png)
Login as the Registered User, and get the accessToken and refresh Token
![Login as the Registered User, and get the accessToken and refresh Token](https://github.com/Lucifer7355/Authentication_Mechanism_Using_Express-Nodejs/blob/main/demonstration_pictures/Screenshot%20(263).png)
Use the accessToken to access “/posts”
![Use the accessToken to access “/posts”](https://github.com/Lucifer7355/Authentication_Mechanism_Using_Express-Nodejs/blob/main/demonstration_pictures/Screenshot%20(264).png)
Once the “accessToken” expires after 15 mins, refresh both tokens by calling the /refresh API (using the unexpired “refreshToken”)
![Once the “accessToken” expires after 15 mins, refresh both tokens by calling the /refresh API (using the unexpired “refreshToken”)](https://github.com/Lucifer7355/Authentication_Mechanism_Using_Express-Nodejs/blob/main/demonstration_pictures/Screenshot%20(265).png)
Finally in order to logout just hit the end point with the current access token which will remove the given token from the list of active user tokens.
# Installation Procedure
Anyone interested in testing the application can follow the following steps to make call to the rest apis.
```
- git clone https://github.com/Lucifer7355/Authentication_Mechanism_Using_Express-Nodejs.git
- cd Authentication_Mechanism_Using_Express-Nodejs
- npm install 
- nodemon authServer.js
- Now open a new terminal shell and run "nodemon validateToken.js" without quotes.
- Open postman or insomnia to make a rest api testing call to the backend.
```