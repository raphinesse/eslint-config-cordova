# eslint-config-cordova
This repository centralizes the ESLint configuration used for Cordova's development.

## Installation

`eslint-config-cordova` comes with all plugins configs and even `eslint` itself. So all you need to do to get started is:

    npm i -D eslint-config-cordova


## Usage
```yml
# In package.json
{
  "scripts": {
    "eslint": "eslint ."
  }
}
```

```yml
# In .eslintrc.yml
root: true
extends: cordova
```

```yml
# In spec/.eslintrc.yml
extends: cordova/node-tests
```

```yml
# In cordova-js-src/.eslintrc.yml
extends: cordova/browser
```

## Reference

This package exposes the following shareable ESLint configurations:

### `cordova/node` (or simply `cordova`)
For linting scripts intended to be run with Node.js.

### `cordova/node-tests`
For linting Jasmine tests of Cordova's Node.js scripts.

### `cordova/browser`
For linting cordova-style CommonJS modules intended to be run in the browser (before they are bundled).

### `cordova/browser-tests`
For linting Jasmine tests of Cordova's browser code.
