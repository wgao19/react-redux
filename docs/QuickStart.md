# Quick Start

[Redux](https://github.com/reduxjs/redux) has no knowledge of [React](https://reactjs.org/). You may create your redux app using other UI rendering frameworks, or not using any frameworks at all.
`react-redux` is the official [React](https://reactjs.org/) binding for [Redux](https://github.com/reduxjs/redux).

## Installation

To create your `react` app with `redux` _and_ `react-redux`:

```
npm install --save react redux react-redux
```

<!-- TODO: add devtools related section -->

## Overview

In summary, `react-redux` provides you the binding to `connect()` your app to the store, which in essence enables you to:

1. Access store from any `connect()`ed components of your app
2. Dispatch actions to your store from any `connect()`ed components of your app

To specify which part of store you will need for such component, you provide a function that is by convention called `mapStateToProps`.
And to specify which actions you will use, you provide a function that is by convention called `mapDispatchToProps`. You will normally call `connect` in this fashion:

```
connect(mapStateToProps, mapDispatchToProps)
```

This will return a function that waits for you to feed in your un`connect()`ed component.
And to obtain your final, `connect()`ed component, you then call this returned function with your `Component`:

```
connect(mapStateToProps, mapDispatchToProps)(Component)
```

## Example

As an example, we create a Todo List app using React and Redux.
Suppose we have our React UI components as follows:

<!-- TODO: React todo list app using internal states -->

```
// placeholder for code snippets of a React todo list app using internal states
```

Placeholder for [Codesandbox](#) link.

Suppose also that we have created this Redux store ready to replace our internal state.
To learn about designing your Redux store, [the official Redux docs](https://redux.js.org/basics) has an excellent guide and we will not cover the same topics here again.

<!-- TODO: Redux store, reducers and actions -->

```
// placeholder for code snippets of our redux store
```

Placeholder for [Codesandbox](#) link.
