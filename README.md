# ReactMobxSSR starter

# Description

Minimalistic Isomorphic TODO list application that benefit of SSR (server side rendering), already set up with:
- React 16 + React Router 4
- MobX 5.5 (state management library) https://github.com/mobxjs/mobx
- Node + Express
- reactive approach to update component state (using ES2016 decorators e.g. @observable, @observer)
- Flow (static type checking at compile time)
- Webpack (livecompiling and HMR) with a configurations for both dev and prod environments
- Unit testing with Jest
- Sass compilation
- Custom VScode config for debugging

# Build and run

Install:
```
yarn install or npm install 
```

Build:
```
npm run build or npm run build:prod //depending on the environment 
```

Run:
```
npm run start or npm run start:prod //depending on the environment 
```

# Description
This app doesn't add any unuseful complexity, just a simple TODO list implemented following the best practice with some useful npm tasks for build and run your app


# Dev and Prod
- the starter comes with two webpack configurations for devevelopment and production environments.
- To speed up the dev environment the app comes with HMR enabled and already configured with Sass Hot reload and React hot loader.

# Coding conventions
- every Class must start with a capital letter.
- unit tests should be placed in the same folder of the component and should following this naming "componentName.test.js" in order to be run automatically by Jest

# Basic folder structure:

- Stores
   * Domain stores:
       stores the data which'll be needed in your app. (user data, for example todos array)
   * View/UI: stores:
       stores the data which'll be needed to present your app (loading, error variables..)
       if the state of the store is too simple there's no need of a specific component ui-store.

- Models: Here you can define the data models

- Services: Here you can make services like api calls, inside singleton with static methods that will be used directly by the stores

- Components: Container or Smart Component, Dumb or presentational component

- Style: any scss must be placed in the style folder and must have the prefix _ if is a partial file

