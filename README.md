# conference-app

:circus_tent: A Sample Conference App built with React Native

> Demo App inspired on [ionic-conference-app](https://github.com/ionic-team/ionic-conference-app)

### Quick start

```bash
# clone repo
$ git clone https://github.com/lexmartinez/conference-app

# change directory to cloned app
$ cd conference-app

# install the dependencies with yarn
$ yarn install

# start react-native (Expo) server with running App
$ yarn start
```

# Table of Contents

* [Dependencies](#dependencies)
* [Developing](#developing)
* [Screenshots](#screenshots)
* [Participate](#participate)
* [License](#license)


 ## Dependencies
 
 You'll need to run this app:
 * `node` and `npm` (Use [NVM](https://github.com/creationix/nvm))
 * Ensure you're running Node (`v8.9.4`+) and NPM (`5.6.0`+)
 * `react-native-cli: 2.0.1`
 * `react-native: 0.54.0`
 
  `conference-app` is a `react-native` mobile application is assumed that you're familiarized with this framework, otherwise it is here where you should start [react-native-getting-started](https://facebook.github.io/react-native/docs/getting-started.html#content)

## Developing
  
With `yarn start` command runs your app in development mode.

Open it in the [Expo app](https://expo.io) on your phone (IOS or Android) to view it. It will reload if you save edits to your files, and you will see build errors and logs in the terminal.

Sometimes you may need to reset or clear the React Native packager's cache. To do so, you can pass the `--reset-cache` flag to the start script:

```
yarn start --reset-cache
```

> For further information regarding app bootstraping and other useful commands see [DETAILS.md](https://github.com/lexmartinez/conference-app/blob/master/DETAILS.md)

## Screenshots

| <img src="https://raw.githubusercontent.com/lexmartinez/conference-app/master/screenshots/screenshot-1.png" width="300"> | <img src="https://raw.githubusercontent.com/lexmartinez/conference-app/master/screenshots/screenshot-2.png" width="300">  | <img src="https://raw.githubusercontent.com/lexmartinez/conference-app/master/screenshots/screenshot-3.png" width="300"> |
| ------------- | ------------- |------------- |
| <img src="https://raw.githubusercontent.com/lexmartinez/conference-app/master/screenshots/screenshot-4.png" width="300"> | <img src="https://raw.githubusercontent.com/lexmartinez/conference-app/master/screenshots/screenshot-5.png" width="300">  | <img src="https://raw.githubusercontent.com/lexmartinez/conference-app/master/screenshots/screenshot-6.png" width="300"> |

## Changelog

### After SDK update from 26.0.0 to 32.0.0

Following the steps in : https://docs.expo.io/versions/latest/workflow/upgrading-expo-sdk-walkthrough/

- Replaced `26.0.0` in `app.json` with `32.0.0`
- Replaced the `react`, `react-native` and `expo` dependencies in the `package.json` file with 
  
  ```
  {
    "react-native": "https://github.com/expo/react-native/archive/sdk-32.0.0.tar.gz",
    "expo": "^32.0.0",
    "react": "16.5.0"
  }
  ```
- Deleted the `node_modules` directory and run `yarn install` 
- Removed this section from the `.babelrc` file :

  ``` 
  "env": {
      "development": {
        "plugins": ["transform-react-jsx-source"]
      }
    }
  ```

  - Changed the scripts in `package.json` to replace `react-native-scripts` with `expo`
  - Removed `node-modules` folder, and ran `npm install` 
