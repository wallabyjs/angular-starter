# Wallaby.js

**To get wallaby.js working** after you have generated your project with `angular-cli`, you'll need to do the following:
- Add the [wallaby.js config file](https://github.com/wallabyjs/angular-starter/blob/master/wallaby.js) to the project.
- Add the [wallaby.js test bootstrap file](https://github.com/wallabyjs/angular-starter/blob/master/config/spec-bundle-wallaby.js) to the project.
- Run `npm install wallaby-webpack electron --save-dev`.

Note that the sample is [using Electron test runner](https://wallabyjs.com/docs/integration/electron.html). 

Alternatively, you may use [Chrome (headless) runner](https://wallabyjs.com/docs/integration/chrome.html). In this case you may  [change the `env` setting in the wallaby config file](https://github.com/wallabyjs/angular-starter/blob/master/wallaby.js) to `env: {kind: 'chrome'}`, and you will not need to `npm i electron` (and can remove `electron` from the `package.json` dependencies). 

You may use PhantomJs runner if you like. In this case you may [remove the `env` setting from the wallaby config file](https://github.com/wallabyjs/angular-starter/blob/master/wallaby.js), and you will not need to `npm i electron` (and can remove `electron` from the `package.json` dependencies).
