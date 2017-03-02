#Monkey in the tree hole#
a little web app i am working on
##The basic structure##
``` html
├── README.md
├── client // Front-end
│   ├── build
│   │   ├── asset-manifest.json
│   │   ├── favicon.ico
│   │   ├── index.html
│   │   └── static
│   │       ├── css
│   │       │   ├── main.9a0fe4f1.css
│   │       │   └── main.9a0fe4f1.css.map
│   │       ├── js
│   │       │   ├── main.478fb047.js
│   │       │   └── main.478fb047.js.map
│   │       └── media
│   │           └── logo.5d5d9eef.svg
│   ├── package.json
│   ├── public
│   │   ├── favicon.ico
│   │   └── index.html
│   ├── src
│   │   ├── App.css
│   │   ├── App.js
│   │   ├── App.test.js
│   │   ├── images
│   │   │   └── logo.svg
│   │   ├── index.css
│   │   └── index.js
│   └── yarn.lock
└── server // express back end (if needed)
    ├── app.js
    ├── index.js
    ├── npm-debug.log
    ├── package.json
    └── yarn.lock
```
##Develpe and Publish##
``` html
// Static nginx serving --------
// just pure front end development@localhost:3000: cd client; yarn run start
// 
// Reverse proxy nginx serving ---------
// back end development@localhost:9000: node server
// publish: cd client; yarn run build; cd ..; node server
// edit nginx.conf to proxy_pass http://127.0.0.1:9000
```
