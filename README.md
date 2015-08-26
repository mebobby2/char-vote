# Tutorial to help me learn react+flux

## Notes
- *babel-node server.js* to start the node server. We will be writing the React components in ECMAScript 6 and will be rendering them on the server, hence we need babel compiler to convert ES6 to ES5. ES5 is used because the older server, where this new server is based upon, was written in ES5. So keeping the server code in ES5 will make it easier to port over.
- *bower*. Do not know why the author decided to use bower as well as npm+browserify. Browserify by itself would have suffice. Anyways, once bower is installed with *npm install*, you can then install the bower components by *node_modules/bower/bin/bower install*
- While in development, run *gulp* from one terminal (to build the js files), and *npm run watch* to restart the nodejs server when files change. Leave these two processes running while you develop.
- Also need to start MongoDB. Create a data dir first *sudo mkdir -p /data/db* and then run *mongod* from the mongo folder.
- To import the newedenfaces.bson into mongo db, run *mongorestore newedenfaces.bson*
- The *postinstall* script inside package.json is for deployment to Heroku. The command compile the app and download Bower packages after deployment.