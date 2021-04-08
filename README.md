# IMDB Demo

<p float="left">
  <img src="../main/promo/home_screen.jpeg" width="250" />
  &nbsp;&nbsp;
  <img src="../main/promo/movie_details.jpeg" width="250" /> 
</p>

## Prerequisites

Before being able to install and run the app, there are some dependencies you will need setup:

- git
- yarn
- nodeJS

To run with the iOS simulator, you will also need:

- ruby
- cocoapods
- XCode

For Android, you will need

- Java JDK
- Android Studio

## Getting Started

#### 1. Clone the repository

```bash
git clone git@github.com:Clecotech/imdb_copy.git
```

#### 2. Install JS dependencies

```bash
yarn global add react-native-cli
yarn install
react-native link
```

For iOS development, you will also need to install the cocoapod dependencies:

```bash
cd ios
pod repo update
pod install
```

#### 3. Run the app

To build and run the iOS app in the simulator

```bash
react-native run-ioS
```

Alternatively, to run the Android version of the app

```bash
react-native run-android
```

## Troubleshooting

### iOS version

If you see the app open on iOS/ANDROID and immediately close, ensure the device/simulator is running
iOS/ANDROID.

### Build fails in iOS

This may be a problem with dependencies not being correctly linked to the xcode project. To fix,
try the following:

```bash
cd ios
pod repo update
pod install

cd ..
react-native link
```

