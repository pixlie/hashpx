# Single page apps
Use ES2015, React, Redux, Immutable and friends to build your user-facing product

## Why build single page apps?
You will want to build single page apps (SPA), with React because:
-  Browsers are powerful devices which do a lot more than just parse the HTML printed from traditional backends
-  User's state management (notifications, counts, errors) can be pushed to the browser
-  For long running apps, there is a lot of processing that you can offload to the browser
-  Backend focuses on data storage, validation and business logic constrainsts
-  Scale either full-stack or separate backend and frontend teams
-  Migrate to native apps using React Native

## Why not build single page apps?
There are certain situations where you might not want to build SPAs:
-  User interaction on your software product is low - you want the user to get whatever they came for as quickly as they can and leave
-  Product is not long running on the browser or mobile devices
-  Users are mostly not on modern browsers
-  Product is native only and you really iOS or Android native apps

## Context
This playbook assumes that you are starting off with the React based stack. We will go from sractch (create-react-app) to add all the necessary parts, including tests. Feel free to jump in and out of sections.

## The setup before the setup
You might want to read on the project startup playbook first if you have not done so. These are what you will need before beginning an actual React based app:
-  Node.js setup on your computer, [prefer LTS versions](https://nodejs.org/en/download/)
-  Install create-react-app in your repository

## Going forward
-  [Get an overview of React based SPA](Overview-of-React-SPA.md)
-  [Get started with your SPA](Start-with-React.md)