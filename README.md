# Welcome to your Expo app 👋

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

## Get started

1. Install dependencies

   ```bash
   npm install
   ```

2. Start the app

   ```bash
    npx expo start
   ```

## Project structure

This project follows the Clean Architecture. You'll find the following folders:

- `/domain`: the entities

  - `/entities`: these are all the TypeScript types for each entity.
  - `/enums`: contains all the enums used in the app.

- `/application`: the business logic of your app

  - `/reducers` : these are the reducers that handle the state of your app.
  - `/usecases` : these are the files where are placed the slices of your state along with actions that act on that slice.
  - `/utils`

- `/infrastructure`:

  - `/api`: the implementation details to access data from a remote source (REST APIs, GraphQL APIs).
  - `/storage`: the implementation details to access data from a local source (SQLite, Realm, AsyncStorage).
  - `/errors`: the implementation details to handle errors.
  - `/logger`: the implementation details to log information about the app.
  - `/notification`: the implementation details to send notifications (Push Notifications, Local Notifications).
  - `/tracking`: the implementation of third party analytics tools (Firebase Analytics, Google Analytics).

- `/ui`: contains the user interface :
  - `/components`: contains the reusable components used across the app.
  - `/screens`: contains the screens of your app.
  - `/navigation`: contains the routes and the navigation logic for each screen.
  - `/theme`: contains the styles that are shared between the UI layer.
  - `/utils`: contains the helpers, constants, etc. that are shared between the UI layer.
  - `/constants`: contains the constants used in the app.
  - `/assets`: contains the images and fonts of your app.
