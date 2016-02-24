FROM davidbebb/nodejs-container:latest
RUN echo '{ "name": "cloud", "version": "0.0.0", "private": true, "scripts": {   "start": "node ./bin/www",   "test": "node ./bin/test" }, "dependencies": {   "async": "^1.5.0",   "bcrypt-nodejs": "0.0.3",   "body-parser": "~1.15.0",   "connect-flash": "~0.1.1",   "cookie-parser": "~1.4.1",   "crypto-js": "^3.1.5",   "debug": "~2.2.0",   "express": "~4.13.4",   "express-session": "^1.0.4",   "jade": "~1.11.0",   "method-override": "~2.3.5",   "moment": "^2.10.6",   "mongodb": "~2.1.7",   "mongoose": "^4.4.4",   "morgan": "~1.7.0",   "node-forge": "^0.6.20",   "nodemailer": "^2.2.1",   "passport": "^0.3.2",   "passport-local": "^1.0.0",   "q": "^1.1.0",   "request": "^2.27.0",   "serve-favicon": "~2.3.0" }, "devDependencies": {   "jasmine": "^2.4.1",   "requires-regex": "^0.3.3",   "selenium-standalone": "^4.8.0",   "selenium-webdriver": "^2.48.2",   "webdriverio": "^3.4.0" }}' > package.json
RUN npm install
RUN npm install -g webdriverio@3.4.0
RUN npm install -g jasmine
RUN npm install -g jasmine-node
RUN npm install -g request
RUN cd node_modules/mongodb
RUN npm install
