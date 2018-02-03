# Overview of a React based SPA
React itself is only part of the ecosystem of software that you will need to build your SPA. Let's see how these all stack up:

## Enter React
-  React is the view layer
-  Uses HTML as the templating laguage
-  You write components which are basically bunch of HTML put together - say user profile sidbar
-  React components can be composed just like you would put `<p>` tag inside `<div>`
-  Composition gives you great power - build large apps out of small components which are resusable
-  Componets can take variables (**props**), that can change what the component displays or does
-  Event handlers (*on-click*, *on-submit*, etc.) are integral part of components - user interaction is at the core

## Enter Redux
-  React props are not supposed to change inside a component (immutable)
-  React components can have another type of variables (**state**) which can change to reflect what the user is doing with the component, like forms
-  Getting this change information across the many components you will have is a mess
-  Enter Redux - you define the application's state (**store**) at a global level and access it from anywhere
-  The state itself should be immutable - which means changes will product new state instead of updating existing one - that is where Immutable.js comes in
-  This enables clear separation of views (HTML based layout) and containers (code that deals with the state and can change the state)
-  Change can also come from AJAX calls (you save form data to backend API, authenticate the user, fetch a  list of friends, etc.)

## Enter Router
-  As you must be thinking - your SPA will slowly get large, how do you combine all the views and containers?
-  Router gives you a well known way to separate your SPA - URL routes, just like in any other web application
-  Integrates well with Redux store and can be changed from within your SPA

## An exmaple to clear the head
-  React **views** (components without interal state) for product list, product view, related products, shopping cart, user profile, user orders, navigation...
-  Redux **store** to keep all the data user requires to go through your awesome T-shirt discovery app
-  **Containers** which attach needed data to the views, or define the methods that allow user to interact (say add T-shirt to favorites)
-  Redux **actions** which connect with the backend, makes AJAX requests to GET, POST, PUT, DELETE, etc.

## Benefits
-  Backend does not care about the user intrinsically - does user have a red icon saying "15 favs" - don't care!
-  Backend is a thin API - RESTful (or otherwise)
-  Backend stores data in relation database
-  Backend tracks that the user is authenticated (logged in)
-  Backend makes sure un-authenticated or un-authorized requests are not allowed
-  SPA takes full care of users' interactions
-  SPA can grab data from multiple backend API endpoints to show a single product page or anything else
-  SPA can change UX depending on browser size or user preference
-  SPA can cache requests as needed