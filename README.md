# FireCMS

![alt="fireCMSlogo"](https://firecms-9763b.firebaseapp.com/images/fireCMS_logo.png)

Open Source CMS with Firebase SDK and ~~Angular~~ VueJS licensed under MIT

> Was an April Fool Joke. But i will get this shit run. Sorry if someone is waiting.

FireCMS is an open source CMS project founded by [SayChunKim](https://github.com/SayChunKim) using [QuillJS](http://quilljs.com), Firebase and ~~Angular~~ Vue (Vue4Life)

~AngularJS aka [AngularFire](https://github.com/firebase/angularfire) (TBA for Angular 2/4 version)~ VueFire


FireCMS is served for balance for simplicity and performance. Simplicity is meant for developers' dilemma for configuring and deploying full-stack enviroments
which fits for multiple platforms. Ideal for engaging users with simple push of `submit` button.

Demo link [here](https://myxlab-76e7d.firebaseapp.com)

FireCMS has supported features included from start:

1. 3-lines of JS for Database Initialization
2. Integrated Authentication using Google/Facebook/Github/Twitter/EmailPassword Authentication
3. Realtime Database via secure request with AngularFire for pages content and metadata
4. User Roles Management (Admin,Editor) for Create/Read/Update/Delete permissions
5. Integrated with Google Analytics for advertising ROI Measurement site monitoring with just provide tracking ID
6. Push Notification using (Firebase Cloud Messaging) for subscriptions*
7. Firebase Hosting with Firebase-CLI

## Getting Started
### Setting Up
1. `git clone` the project and allocate to your project folder, in same time go [console.firebase.google.com](https://console.firebase.google.com) to make your project
2. Install `npm` and `firebase-cli` into Terminal/CMD via [tutorial here]() 
3. Open Terminal `firebase init` under your folder project to initialize your Firebase Project 
4. Go to project root folder > index.html and add the web app script snippet given by Firebase Console before end of `<body>` tag
5. **[UPDATE COMING SOON] :placeholder "The fun begins here"**.  I will upload the VueFire project structure (public + admin) here. Stay tuned.


NOTE: this is just snippet, please refer Firebase Console.
```    <script src="https://www.gstatic.com/firebasejs/3.7.4/firebase.js"></script>
       <script>
          // Initialize Firebase
          var config = {
          apiKey: "xxxxxxxxxxxxxxxxxxxxxxxxx",
          authDomain: "xxxxx.firebaseapp.com",
          databaseURL: "https://xxx.firebaseio.com",
          projectId: "xxx-1234",
          storageBucket: "xxxx.appspot.com",
           messagingSenderId: "xxxxx"
          };
          firebase.initializeApp(config);
      </script>
```
6. Terminal type `firebase serve` for localhosting.
7. For the first time, login with the method you have chosen. You will be redirected to admin homepage if successfully authenticated.
8. Enjoy. Let's Start writing your first post !


### Authentication
1. Go to [console.firebase.google.com](https://console.firebase.google.com) of your project and select **Authentication > Sign-In Method** to enable your Auth.
2. May add other authentication method via FireCMS > Setting section
3. If forgot password from logging in, just go 'Forgot Password' section and insert your `email_id` to reset your password.

### Database
FireCMS helps you to add/arrange posts and your contents secured with Firebase Realtime noSQL Database in JSON format with security.

### Push Notifications
Firebase Cloud Messaging helps engaging users/clients via subcription methods similarly as Google Cloud Platform. FireCMS helps engaging Web via [Service Worker](https://developers.google.com/web/fundamentals/getting-started/primers/service-workers), Android and iOS via FCM SDK
* Do note this feature requires secured application server keys which is not applicable for static site hosting services.

### Hosting
1. Using Firebase-Cli, you may deploy your site via Terminal, exit via Ctrl+Z if `firebase serve`
2. `firebase deploy` (make sure your site folder under 'public' folder !)
3. `firebase open` for opening site automatically or just got to the URL given

> Star this repository if you'd love to see this happen or enjoyed reading !

*Sincerely,*<br>
*SC Kim*
Potato Developer
