# frontend-webpack-boilerplate

## Why ?
One may think this is yet another webpack-based boilerplate for front-end development. However, most of these projects are suited to the developer's way of working. Some don't use Sass, some don't care about loading images or fonts, others have ESLint installed globally, etc. This is my own boilerplate, which includes pretty much everything I use and makes my life easier.

## How does this work ?
There are 2 Webpack configs: one for development and one for production. Webpack supports a [Mode flag](https://webpack.js.org/configuration/mode/) which changes the "base" config behind the scenes. This includes optimization and plugins, to name a few.

Both configs share core functionality:
- JavaScript bundling and transpiling.
- Loading styles, images and fonts.
- Injecting tags into HTML

The development config includes a DevServer with [HMR](https://webpack.js.org/concepts/hot-module-replacement/) to improve the development experience. It also includes source-maps for both javascript and styles.

The production config includes an uglifier and enables html/css minification.

## What else is included ?
Styling tools are also included: ESLint and Prettier. You can change the default config of both tools by editing the `.eslintrc.json` file.

## What's missing ?
Pre-commit hooks (using Husky)