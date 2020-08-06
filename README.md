<h1 align="center">🌚 React Design Dark Theme 🌚</h1>

<div align="center">

Dark theme [variables](https://github.com/machinaai/dark-theme/blob/master/index.ts).


<span>Visit <a href="https://designer.reboot.vc" target="_blank">https://designer.reboot.vc</a> to preview.</span>

![](https://raw.githubusercontent.com/machinaai/logos/master/dark-theme/dark-theme.png)

</div>

## Install

```bash
$ npm install @machinaai/dark-theme
```

## Usage

```js
import darkTheme from '@machinaai/dark-theme';

// webpack.config.js: less-loader
{
  loader: 'less-loader',
  options: {
    modifyVars: darkTheme,
  },
},
```

Use in React Designer.

There are two main methods:

Method 1:
On "front" project edit the file config/config.ts
```js
import darkTheme from '@machinaai/dark-theme'';    //<-- Add this line abobe in the file

//Locate the following block
theme: {
     ...darkTheme,  //<-- Uncomment this line
    'primary-color': defaultSettings.primaryColor,
  },
```

Method 2:
Add the following dependency to package.json
```
"umi-plugin-antd-theme": "2.1.2"
```
This will enable the Theme in the Drawer
