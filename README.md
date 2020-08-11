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
- run react app (extensions files) on the browser `npm run start`
- build unpacked extension `npm run build`
- production build (this zip file can upload to Google WebStore) `npm run pack`
- goto: `chrome://extensions` in the browser and enable `'developer mode'`
- press `Load unpacked` and target the folder `build/`

The project is automatically being watched, any changes to the files will recompile the project.

**NOTE**: changes to the **content page** and **background page** scripts requires you to reload the extension in `chrome://extensions`

![alt text](https://snipboard.io/1W2m0H.jpg 'React Chrome Popup')

## Build/package for production

- update version number inside `./src/manifest.json`
- run `npm run pack`
- upload `extension-build.zip` to the chrome webstore.

This will run a production build and will automatically zip it as an extension package in the root folder named: `extension-build.zip`

## React folder

This folder contains the react single app source code.
inside it can build page for popup, options, tabs.

see: `./src/`

## Chrome folder

This `./build` folder contains the content page,background page, popup page scripts.
