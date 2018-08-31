<B>Five Steps to deploy STRAPPD in your local community to help Homeless people find resources close to them.</B>

1. Install <a href = "https://nodejs.org/en/download/"> Node.js</a>, <a href = "https://cordova.apache.org/">Cordova</a>(npm -g install cordova ), <a href = "https://ionicframework.com/getting-started">Ionic</a>(npm install -g ionic@1.6.0 ), <a href = "https://bower.io/">Bower</a>(npm install -g bower) & <a href = "https://gulpjs.com/">Gulp</a>(npm install -g gulp). 

2. Signup for <a href="https://accounts.google.com/signup">Google account</a>, add <a href="https://console.firebase.google.com">New Firebase Project</a>, Create a <a href="https://firebase.google.com/docs/database/">Realtime Database</a> & Import <a href="">testdata</a> into databse. Please make sure to enable the Email/Password in the Sign-in Method Tab under Authentication tab in Firebase console.

3. Update the https://yourproject.firebaseio.com/ variable at line 1(“var refurl”) in www/js/app.js with your RealTime Database Link from firebase console.

4. Replace script at lines 30-42 in www/index.html with <a href="https://firebase.google.com/docs/web/setup">WebSetup code</a> from firebase console in Authentication tab. Also, change the “YOUR_API_KEY” value at line 90 with your <a href="https://developers.google.com/maps/documentation/javascript/get-api-key">Google Maps API key</a>. 

5. To <a href="https://firebase.google.com/docs/hosting/">Host the web app</a> on Firebase, Install <a href="https://firebase.google.com/docs/cli/">Firebase CLI</a>(npm install -g firebase tools), firebase login & init in project folder, install npm dependencies, select www as public directory and run Firebase Deploy. 


You can also add <a href="https://analytics.google.com/analytics/web">Google Analytics</a> to the index.html head tag to get Analytics Info about the app.