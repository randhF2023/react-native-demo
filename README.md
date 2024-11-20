# React Native & Expo Initial Setup

Install nodejs v22 (I used 22.8.0).

Create an expo app (use latest or 3.1.1):

```
npx create-expo-app@latest
```

Follow the prompts to name and create your project.

NOTE: If on MacOS, you may have to also install `watchman`, e.g. using brew:

```
brew install watchman
```

The version I have installed is `2024.11.18.00` (probably latest).

At this point, you should be able to start a "development server":

```
cd <project-name> && npx expo start
```

In addition to starting the development server, this opens a CLI
that you can poke around in.

# Viewing On a Native Platform

There are a couple ways to natively develop for the mobile platforms
(Android, iOS), but it seems to me that using the Expo Go app is the
most complete.

1. Create an account on https://expo.dev/
2. Login on your computer using the CLI:
    ```
    npx expo login
    ```
3. Download the Expo Go app on your phone (iOS or Android) and log in.

Now when you start the development server on your computer, you should
be able to connect to the development server through your mobile app.

Note that the first time you connect via web or mobile app, expo will
automatically install dependencies for your target platform, so it will
take a few seconds.

More instructions / debugging help here: https://docs.expo.dev/get-started/start-developing/
