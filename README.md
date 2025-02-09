# Monaco Editor for Eclipse Dirigible

## Overview

Monaco Plugin for the [Eclipse Dirigible](https://github.com/eclipse/dirigible) WebIDE v3.x and above.

Build the [Eclipse Dirigible](https://github.com/eclipse/dirigible), deploy on e.g. Tomcat Web Container and go to location:

> http://localhost:8080/services/v4/web/ide-monaco/editor.html

## Used libraries

This module uses some third party libraries.

- [Monaco editor](https://github.com/dirigiblelabs/monaco-editor)
- [acorn.js](https://github.com/acornjs/acorn)
- [css-format-monaco](https://github.com/troy351/css-format-monaco/)

## Update

To update the Monaco version:

1. Go to [dirigiblelabs/monaco-editor](https://github.com/dirigiblelabs/monaco-editor)
1. Fetch the latest changes from the original repository
1. Run `npm run release`
1. Copy the release artefacts from the `release` folder
1. Replace the content of [ide-monaco/monaco-editor](https://github.com/dirigiblelabs/ide-monaco/tree/master/ide-monaco/monaco-editor) with the content from the `release` folder

To update the css-format-monaco version:

1. Get the latest version - `npm i css-format-monaco`
2. Go to `node_modules/css-format-monaco/dist/`
3. Copy `css-format-monaco.min.js`
4. Paste/replace it in `ide-monaco/js/formatters/`

## License

Forked from: [Monaco](https://github.com/Microsoft/monaco-editor)
