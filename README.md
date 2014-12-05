[![Build Status](http://198.199.100.206:8080/buildStatus/icon?job=unit-tests)](http://198.199.100.206:8080/job/unit-tests/)

##NodeJS Against Humanity

Orignally from: <a href="https://github.com/amirrajan/nodejs-against-humanity">Amir Rajan - NodeJS Against Humanity</a>

I did not fork the original project because I wanted to be able to showcase a CI/CD flow and couldn't with the github fork model.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/2.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/2.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/2.0/">Creative Commons Attribution-NonCommercial-ShareAlike 2.0 Generic License</a>.

NodeJS implementation of Cards Against Humanity. Here's a screenshot:

<img src="/nodejs-against-humanity.png" />

##Run Locally

Install all the dependencies:

    npm install (you may need to prefix this with sudo if you're on Mac)

Run the app:

    node server.js

Then navigate to `http://localhost:3000`

If you want tests to execute every time you change a file:

    jasmine-node --junitreport spec/
    
Docker Commands

    sudo docker build -t sabind/nodejs-against-humanity:master .
    sudo docker run -d -p 3000:3000 --name sample-app sabind/nodejs-against-humanity:master start
    
    
BUILD the PR