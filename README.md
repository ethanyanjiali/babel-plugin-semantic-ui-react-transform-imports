# babel-plugin-semantic-ui-react-transform-imports

Forked from [babel-plugin-transform-semantic-ui-react-imports](https://github.com/skleeschulte/babel-plugin-transform-semantic-ui-react-imports/blob/master/README.md)

This version supports Babel 7 by fixing a bug in index.js. The original one only supports up to Babel 6. Thanks @tcrossland for contributing the bugfix

This plugin is renamed to `semantic-ui-react-transform-imports` and published to npm as [babel-plugin-semantic-ui-react-transform-imports](https://www.npmjs.com/package/babel-plugin-semantic-ui-react-transform-imports)


## Function

This plugin can convert module imports from `semantic-ui-react` to
default imports. Example:

    // Input:
    import { Button, Container } from 'semantic-ui-react';

    // Output:
    import Button from 'semantic-ui-react/dist/es/elements/Button/Button.js';
    import Container from 'semantic-ui-react/dist/es/elements/Container/Container.js';


## Installation

    npm install babel-plugin-semantic-ui-react-transform-imports --save-dev

Depending on how you use the plugin, you also need to install
[semantic-ui-react](https://www.npmjs.com/package/semantic-ui-react),
[semantic-ui-css](https://www.npmjs.com/package/semantic-ui-css) and/or
[semantic-ui-less](https://www.npmjs.com/package/semantic-ui-less) (see
below).

## Usage

Add the plugin to your Babel configuration (e.g. in .babelrc):

    {
        "plugins": ["semantic-ui-react-transform-imports"]
    }
    
## More

[Original Documentation](https://github.com/skleeschulte/babel-plugin-transform-semantic-ui-react-imports/blob/master/README.md)
