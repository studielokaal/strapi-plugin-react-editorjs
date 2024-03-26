<div align="center">
    <img alt="Logo" src="https://github.com/melishev/strapi-plugin-editor-js/blob/master/.github/assets/strapi-plugin-editorjs.png" width="400px">
</div>

<h1 align="center">🎛 Strapi + ✒️ Editor.js</h1>

⚠️ **This is a Strapi v4 version of this plugin! In order to use with v3, please use [release v.1.5.1](https://github.com/melishev/strapi-plugin-react-editorjs/releases/tag/v1.5.1).**


## 🙉 What it is?

#### This is a plugin for [Strapi Headless CMS](https://strapi.io) that replaces the standard wysiwyg editor with the cool [Editor.js](https://editorjs.io) and all its compatible add-ons. It is fork of https://github.com/melishev/strapi-plugin-editor-js (the original github repository) with minor changes, i.e. removing the max version compatible version number of nodejs in package.json. Use this package at your own risk (on an as-is basis), we are not planning to develop it and we make no promises w.r.t to maintainance. There is no warranty whatsoever. We hope someone else will maintain a new fork of the original github repository.
<br>

<img src="https://github.com/melishev/strapi-plugin-editor-js/blob/master/.github/assets/strapi-plugin-editorjs.gif">
<br>

## 🍀 Supported official add-ons

This fork does not support add-ons (we make no promises that anything works, see the original repo for a list of add-ons)

## 🤟🏻 Getting Started

```bash
yarn add strapi-plugin-react-editorjs
# or
npm install strapi-plugin-react-editorjs
```

In order for Strapi to show the Link Tool thumbnails correctly, you will need to edit the 'strapi::security' line in ./config/middlewares.js. Change that line to the following (do this at your own risk). 

```js
module.exports = [
  // ...
  {
    name: 'strapi::security',
    config: {
      contentSecurityPolicy: {
        directives: {
          'img-src': ['*'],
        },
      }
    },
  },
  // ...
];
```

<br>

## ⚙️ How to extend/develop this plugin (optional)

The original repository is archived. This repository does not accept pull requests ((high impact, great quality) pull requests are welcome, but don't expect us to do actually merge anything)

Further instructions can be found in the original github repository


### Please note that the add-ons are configured for Strapi, be careful when changing the configuration.

<br>


## ⭐️ Show your support

Give the (original) github repo a star if this project helped you
