# Start with a React application
Assuming that you have the base project setup, and the needed pre-requisites, simply do the following:
```
cd my-project
create-react-app webapp
```

Inside the webapp folder you will have an `src` folder. That is where we will add our actual web application (SPA). Look at the example that has been created for you and run the server `npm run` as per the documentation.

Once you have peek, let's start adding some skeleton to get started:
-  Build a basic Bootstrap based layout
-  Navbar can be separate from the inner page
-  Inner page layout may differ for logged in and logged out users
-  Start with a basic form and simply handle it (without authentication to begin with)


## Install the React ecosystem modules
To build a real application you will need a few modules:
-  Redux for the data (store) management
-  Redux Thunk to allow Redux to handle AJAX requests
-  React Router for URL routes to access many parts of the webapp
-  Immutable for have immutable data store for Redux
-  Command: `npm install --save redux react-redux react-router-dom immutable redux-thunk`

## Highly recommended
We highly recommend you to add some basic tests, we will show you how. For that you need:
-  Jest
-  Command: `npm install --save jest`


## Default project layout
Writing with React components, Redux containers and reducers becomes quite verbose. Initally you want to focus on getting the user interaction flow built quickly and then look into customizing in detail. With that is mind we suggest:
-  Have generic containers for lists, single items and forms
-  Have generic reducers for lists, single items and forms
-  Have actions for AJAX requests for CRUD operations that work well with the above points