# OpenMTP | Android File Transfer for macOS

Version: 1.0.0

Author: [Ganesh Rathinavel](https://www.linkedin.com/in/ganeshrvel "Ganesh Rathinavel")

License: MIT

Requirements: node.js v10, yarn

URL: [https://github.com/ganeshrvel/openmtp](https://github.com/ganeshrvel/openmtp "https://github.com/ganeshrvel/openmtp")



### Download
 The latest dmg file is available on [GitHub Releases](https://github.com/ganeshrvel/openmtp/releases "GitHub Releases")



##### Advanced MTP File transfer application for macOS.

 Transferring files between macOS and Android Devices or any other MTP devices has always been a nightmare. There are a few MTP apps which are available online but most of them are either too expensive or too uncomfortable to use. The official "Android File Transfer" app for macOS from Google has a lot of bugs and limitations, some of which includes not being able to transfer files larger than 4GB, frequent disconnections, unable to rename the folders or files on the android devices. Most of the other apps available online are too expensive and all of them uses either WiFi or ADB protocol to transfer the files, which by the way is really painful to watch.

 All the above-mentioned reasons have prompted me to create an application on my own which will be available FREE to all and FOREVER.

### Features
- Plug and Play. No hassles, easy and instant connection.
- Connected via USB cable, hence providing the highest data transfer rates possible.
- Transfer files which are larger than 4GB.
- Can select between Internal Memory and SD Card.
- Split pane views for both Local Computer and MTP device.
- Grid and List views are available (check Settings).
- Drag n Drop and the other advanced File Manager features are available.
- Transparent, OpenSource and we care for your privacy.
- It's FREE and shall ALWAYS remain FREE!!


## Building from the Source

### Clone
```shell
$ git clone --depth=1 https://github.com/ganeshrvel/openmtp.git

$ cd openmtp
```

[Install Yarn package manager](https://yarnpkg.com/lang/en/docs/install/ "Install Yarn package manager")

```shell
$ yarn
```

### Run
A fresh clone might throw *undefined state* error. Run the commands below, just once, to fix the issue.

```shell
# For Mac and Linux
$ UPGRADE_EXTENSIONS=1 npm run dev

# For Windows
$ set UPGRADE_EXTENSIONS=1 && npm run dev
```

```shell
# Development
$ yarn dev

# Pre-production
$ yarn start

```

### Package

Setup the *code signing* to build, package and publish the app.

Instructions: [https://www.electron.build/code-signing](https://www.electron.build/code-signing "https://www.electron.build/code-signing")

```shell
$ export GH_TOKEN="<github token>"
```

```shell
# For local platform
$ yarn package

# For Multi platform
$ yarn package-all
```

### Technical Features
- Built using Electron v4, React v16.4, Redux v4, Webpack v4, Babel v7 and Material UI v3.8
- Hot module Reload (HMR) for instant feedback.
- Highly modular.
- Inbuilt error logging and profile/settings management.
- Loadables, Dynamic Reducer Injection, Selectors for efficient Code. splitting and performance/startup optimisation.
- Industry standard State management.
- JSS, SASS/SCSS styling.
- Port assigned: **4642**
- *Prettier* is used for maintaining code standards.

### Configurations
- *config/env/env.dev.js* and *config/env/env.prod.js* contains the PORT number of the app.
- *config/dev-app-update.yml* file holds the GitHub repo variables required by *electron-updater*.
- *config/google-analytics-key.js* file contains the Google Analytics Tracking ID.
- *package.json* **build.publish** object holds the values for publishing the packaged application.
- *app/constants* folder contains all the constants required by the app.

### Accolades and Credits

- My sincere thanks to [Vladimir Menshakov](https://github.com/whoozle "Vladimir Menshakov") for the fantastic C++ library and for all the help and support that were extended towards this project.

- This boilerplate is built upon [https://github.com/ganeshrvel/electron-react-redux-advanced-boilerplate](https://github.com/ganeshrvel/electron-react-redux-advanced-boilerplate "https://github.com/ganeshrvel/electron-react-redux-advanced-boilerplate") which is a heavily modified fork of [https://github.com/electron-react-boilerplate/electron-react-boilerplate](https://github.com/electron-react-boilerplate/electron-react-boilerplate "https://github.com/electron-react-boilerplate/electron-react-boilerplate")


 - The app icons were made by [Prosymbols](https://www.flaticon.com/authors/prosymbols "Prosymbols"), [Nikita Golubev](https://www.flaticon.com/authors/nikita-golubev "Nikita Golubev"), [Those Icons](https://www.flaticon.com/authors/those-icons "Those Icons"), [Kiranshastry](https://www.flaticon.com/authors/kiranshastry "Kiranshastry"), [Elias Bikbulatov](https://www.flaticon.com/authors/elias-bikbulatov "Elias Bikbulatov") & [Pixel perfect](https://www.flaticon.com/authors/pixel-perfect "Pixel perfect") and were distributed by [www.flaticon.com](https://www.flaticon.com/ "Flaticon") which is licensed under [CC 3.0 BY](http://creativecommons.org/licenses/by/3.0/ "Creative Commons BY 3.0")
 
- The "no image found" icon was made by Phonlaphat Thongsriphong from [https://www.iconfinder.com/phatpc](https://www.iconfinder.com/phatpc "https://www.iconfinder.com/phatpc")
 
### Debugging
 
\# **Debugging Guide**

[https://github.com/electron-react-boilerplate/electron-react-boilerplate/issues/400](https://github.com/electron-react-boilerplate/electron-react-boilerplate/issues/400 "Debugging Guide")

\# **Dispatching redux actions from main process**

[https://github.com/electron-react-boilerplate/electron-react-boilerplate/issues/118](https://github.com/electron-react-boilerplate/electron-react-boilerplate/issues/118 "https://github.com/electron-react-boilerplate/electron-react-boilerplate/issues/118")

[https://github.com/electron-react-boilerplate/electron-react-boilerplate/issues/108](https://github.com/electron-react-boilerplate/electron-react-boilerplate/issues/108 "https://github.com/electron-react-boilerplate/electron-react-boilerplate/issues/108")

\# **VM112:2 Uncaught TypeError: Cannot read property 'state' of undefined error**

```shell
# For Mac and Linux
$ UPGRADE_EXTENSIONS=1 npm run dev

# For Windows
$ set UPGRADE_EXTENSIONS=1 && npm run dev
```
