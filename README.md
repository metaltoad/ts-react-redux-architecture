
# React TypeScript Architecture

This software repository is a [several part series](https://github.com/keelz/ts-react-redux-architecture). Each branch of this repository provides specific information, code examples, thoughts, and notes regarding the implementations of different libraries and design patterns common within the [TypeScript](https://www.typescriptlang.org/) and [React](https://reactjs.org/) development community.

My motivation for developing this repository originates from a growing community outcry for more. There are countless walkthroughs, blogs, and tutorials showcasing these technologies. What is missing within that endless swirl of information is a repository of information that dives into the deeper concepts of implementations using real-world type examples as source material. My goal is to fill that gap.

After developing several production apps with [TypeScript](https://www.typescriptlang.org/) and the [React](https://reactjs.org/) framework library, I decided to organize my personal notes and experiences into a slightly opinionated library of applications. I will try very hard not to focus too hard on my own opinions, however, many of the design patterns that I will describe within this series are born from opinions of good software development. I humbly ask for your understanding and collaboration!

## Repository Index

* [Master Branch](https://github.com/keelz/ts-react-redux-architecture#react-typescript-architecture)<br />
_install, bootstrap, and configure_

* [Bootstrapping Redux](#bootstrapping-redux)<br />
_install, configure, and test a redux implmentation_

## Branch Index

* [1.0 Description](#description)
* [2.0 Install the Redux Library](#install-the-redux-library)
* [3.0 Install the redux-thunk Middleware Library](#install-the-redux-thunk-middleware-library)
* [4.0 Model the RootState Interface](#model-the-rootstate-interface)
* [5.0 Configure the RootState Service Provider](#configure-the-rootstate-provider)
* [6.0 Configure the Store Service Provider](#configure-the-store-service-provider)
* [7.0 Bootstrap the Store into the App Component](#bootstrap-the-store-into-the-app-component)
* [8.0 Boilerplate the App state reducer](#boilerplate-the-app-state-reducer)
* [9.0 Conclusion](#conclusion)

## Bootstrapping Redux

This article showcases the implementation of the [Redux](https://redux.js.org/) state management library within a [TypeScript](https://www.typescriptlang.org/) client application using the [React](https://reactjs.org/) framework. The architecture for this application is a reflection of the project produced in the [first part of this series](https://github.com/keelz/ts-react-redux-architecture#description).

> __* NOTE *__
>
> There are a number of different state management libraries and utilities written in both JavaScript and TypeScript that support the React framework. The React framework itself provides us with a few different options to manage state that we will most likely cover within these articles.
>
> State management decisions should be made considering the requirements of the application being developed. If your application is smaller and requires highly detailed component level management then [MobX](https://mobx.js.org/) or the [React Context API](https://reactjs.org/docs/context.html) may be good options. Redux, on the other hand, is a good solution for larger applications required to persist and manage application state within multiple namespaces serving many different views. State management decisions should not be taken lightly and a great deal of care should be given to the decision.

### Problem

We need to modify an existing [Single Page Application (SPA)](https://en.wikipedia.org/wiki/Single-page_application) with the following acceptance criteria:

1. Our application will support application state management with the Redux library.
2. Our application will support state dispatch functions (dispatchers) written using a [thunk](https://en.wikipedia.org/wiki/Thunk) design pattern.
3. All application components should have access to state management services.

### Solution

1. Install the Redux library
2. Install the [redux-thunk](https://www.npmjs.com/package/redux-thunk) middleware library.
3. Model the RootState Interface.
4. Configure the RootState service provider.
5. Configure the store service provider.
6. Bootstrap the root state instance into our Application component root.
7. Boilerplate an App state reducer.

### Development Environment Requirements

* [nodejs](https://nodejs.org/en/)
* [A modern IDE](https://code.visualstudio.com/) and [linting utility](https://marketplace.visualstudio.com/items?itemName=eg2.tslint)

## Install the Redux Library
_todo_

## Install the redux-thunk middleware library
_todo_

## Model the RootState Interface
_todo_

## Configure the RootState Service Provider
_todo_

## Configure the Store Service Provider
_todo_

## Bootstrap the Store Into the App Component
_todo_

## Boilerplate the App state reducer
_todo_

## Conclusion
_todo_

__Test our project:__

```
npm run test -- --coverage

---------------------------|----------|----------|----------|----------|-------------------|
File                       |  % Stmts | % Branch |  % Funcs |  % Lines | Uncovered Line #s |
---------------------------|----------|----------|----------|----------|-------------------|
All files                  |       18 |        0 |    11.76 |    16.33 |                   |
 src                       |        0 |        0 |        0 |        0 |                   |
  index.tsx                |        0 |      100 |      100 |        0 |    1,2,3,4,5,7,11 |
  registerServiceWorker.ts |        0 |        0 |        0 |        0 |... 17,118,119,120 |
 src/components/App        |      100 |      100 |      100 |      100 |                   |
  index.tsx                |      100 |      100 |      100 |      100 |                   |
---------------------------|----------|----------|----------|----------|-------------------|
Test Suites: 1 passed, 1 total
Tests:       1 passed, 1 total
Snapshots:   0 total
Time:        2.649s
Ran all test suites.
```

__Build our project:__

```
npm run build
```

__Start our project:__

```
npm run start
```
