# Partials HTML Webpack Plugin

## Installation

Not yet published to npm, install via Github for for now:
```
npm add https://github.com/colbyfayock/html-webpack-partials-plugin --save-dev
```
or
```
yarn add https://github.com/colbyfayock/html-webpack-partials-plugin -D
```

## Usage

Require the plugin in your webpack config:
```
const HtmlWebpackPartialsPlugin = require('html-webpack-partials-plugin');
```

Add the plugin to your webpack config as follows:
```
plugins: [
  new HtmlWebpackPartialsPlugin({
    path: './path/to/partials/body.html'
  })
]
```

### Settings
| Name      | Type     | Default | Description
| path      | String   | none    | Partial location
| inject    | Boolean  | true    | Conditionally inject your partial
| location  | String   | "body"  | HTML tag name where the the partial gets added
| priority  | String   | "low"   | "high" or "low" - determines if the partial gets added from the start of the location or end
| options   | Object   | {}      | Local variables to the given partial
