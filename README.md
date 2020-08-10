# generate-chrome-extension
Boilerplate for Custom Chrome Extensions

[![npm-release](https://img.shields.io/npm/v/generate-chrome-extension.svg?label=npm)](https://www.npmjs.com/package/generate-chrome-extension)
[![generate-chrome-extension](https://github.com/JithinAntony4/generate-chrome-extension/workflows/generate-chrome-extension/badge.svg?branch=master)](https://github.com/generate-chrome-extension)
[![license](https://img.shields.io/npm/l/generate-chrome-extension)](https://github.com/JithinAntony4/generate-chrome-extension/blob/master/LICENSE)
![npm](https://img.shields.io/npm/dw/generate-chrome-extension)
Easily create Google Chrome Extensions using the `latest` version of React.

The following scenarios/options are supported:

- Popup &#10003;
- New Tab &#10003;
- Options &#10003;
- Background Page &#10003;
- Content Page &#10003;

## How to install

```bash
npm install -g generate-chrome-extension
```

## Start creating a new project

```bash
react-chrome
```

![alt text](https://snipboard.io/v4VHAx.jpg 'react-chrome CLI')

## How to use/develop

- change directory to your newly created project
- run react app on the browser(popup.html) `npm run start:react`
- run production build `npm run build:production`
- run extension build `npm run build:extension`
- goto: `chrome://extensions` in the browser and enable `'developer mode'`
- press `Load unpacked` and target the folder `dist/chrome`

The project is automatically being watched, any changes to the files will recompile the project.

**NOTE**: changes to the **content page** and **background page** scripts requires you to reload the extension in `chrome://extensions`

![alt text](https://snipboard.io/1W2m0H.jpg 'React Chrome Popup')

## Build/package for production

- Under developing

## React folder

This folder contains the react single app source code.
Only one feature (popup) lives inside it other features (options,tab) will come soon.

see: `./react/src/App.js`

## Chrome folder

This folder contains the content page/background page scripts.
