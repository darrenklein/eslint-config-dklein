# Overview
This repo serves as the shared set of ESLint configuration rules for JavaScript projects. There are many preferences for JavaScript styles, and this is mine.


# Installation
Make sure your app has included ESLint as a dependency - https://www.npmjs.com/package/eslint

In order to use the rules included here, you must include this repo in your app's dependencies. If your app has a `package.json` file, add it to `devDependencies` and install it by running

    $ npm install --save-dev https://github.com/darrenklein/eslint-config-dklein.git#master

and then run

    $ npm install


# Use
Locally, you will need a `.eslintrc` file to handle your app's ESLint configuration. The app's copy of the `.eslint` file can contain any configuration that is specific to that app, to which our master set of rules will be added.

In your local `.eslintrc` file, add this set of shared rules via the `extends` property:

    "extends": "eslint-config-dklein"

or

    "extends": ["eslint-config-dklein", "plugin:react/all"]

if you need more than one option in the `extends` property.


# Notes
For more info about shared configurations, see https://eslint.org/docs/developer-guide/shareable-configs