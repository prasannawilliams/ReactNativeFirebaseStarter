
---

A basic react native app based off the starter code from (https://github.com/invertase/react-native-firebase)

---
### Getting Started

> If you're only developing for one platform you can ignore the steps below that are tagged with the platform you don't require.

#### 1) Clone & Install Dependencies

- 1.1) `git clone https://github.com/corbinbalzan/ReactNativeFirebaseStarter.git`
- 1.2) `cd reactnativefirebasestarter` - cd into your newly created project directory.
- 1.3) Install NPM packages with your package manager of choice - i.e run `yarn` or `npm install`
- 1.4) `npm install --save `
- 1.5) `react-native link`

#### 2) Rename Project

**You will need to be running Node version 7.6 or greater for the rename functionality to work**

- 2.1) `npm run rename` - you'll be prompted to enter a project name and company name
- 2.2) Note down the package name value - you'll need this when setting up your Firebase project

#### 3) **[iOS]** Install Pods

- 3.1) `cd ios` and run `pod install` - if you don't have CocoaPods you can follow [these instructions](https://guides.cocoapods.org/using/getting-started.html#getting-started) to install it.

#### 4) Add `Google Services` files (plist & JSON)

- 4.1) **[iOS]** Follow the `add firebase to your app` instructions [here](https://firebase.google.com/docs/ios/setup#add_firebase_to_your_app) to generate your `GoogleService-Info.plist` file if you haven't done so already - use the package name generated previously as your `iOS bundle ID`.
- 4.2) **[iOS]** Place this file in the `ios/` directory of your project.
  - Once added to the directory, add the file to your Xcode project using 'File > Add Files to "[YOUR APP NAME]"…' and selecting the plist file.
- 4.3) **[Android]** Follow the `manually add firebase` to your app instructions [here](https://firebase.google.com/docs/android/setup#manually_add_firebase) to generate your `google-services.json` file if you haven't done so already - use the package name generated previously as your `Android package name`.
- 4.4) **[Android]** Place this file in the `android/app/` directory of your project.



On xcode projects add additional command below to generate the main jsbundle

```
npm run build:ios
```

After this open up the .xcworkspace not the .xcodeproj


# Error Notes: 

### Pod related errors: 
``` pod install ```

### npm install error

```
rm -r node_modules
npm cache clean --force
npm install
```



