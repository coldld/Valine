npm install autoprefixer@7.1.1 babel-core@6.25.0 babel-loader@7.1.1 babel-plugin-transform-runtime@6.23.0 babel-preset-env@1.6.0 babel-preset-es2015@6.22.0 css-loader@0.28.4 exports-loader@0.6.4 file-loader@0.11.2 node-sass@4.5.3 postcss-loader@2.0.6 sass-loader@6.0.6 style-loader@0.18.2 url-loader@0.5.9 webpack@2.7.0 webpack-cli@3.3.12 webpack-dev-server@2.7.1 babel@6.23.0 leancloud-storage@4.6.1 marked@0.6.1 source-map@0.5.6 string-format@2.0.0 xss@1.0.3 --save

npm install webpack@2.7.0


dist文件夹：用于存放打包的文件
src文件夹：用于存放我们写的源文件
index.html:浏览器打开展示的首页html
package.json:通过npm init生成的，npm包管理的文件

cmd输入 webpack即可打包

打包后去dist目录 输入 npm publish 发布包



-------------------------------------------------------------------------

![](./src/images/logo.opacity.png)
# Valine  
[![version](https://img.shields.io/github/release/xCss/Valine.svg?style=flat-square)](https://github.com/xCss/Valine/releases) [![npm downloads](https://img.shields.io/npm/dt/valine.svg?style=flat-square)](https://www.npmjs.com/package/valine) [![build](https://img.shields.io/circleci/project/github/xCss/Valine/master.svg?style=flat-square)](https://circleci.com/gh/xCss/Valine) [![donate](https://img.shields.io/badge/$-donate-ff69b4.svg?maxAge=2592000&style=flat-square)](#donate)  

> A simple comment system based on Leancloud.  


[中文教程](https://deserts.io/diy-a-comment-system/)

- High speed.
- Safe by default.
- Easy to customize.
- No server-side implementation.
- Support part of the markdown syntax.

**Table of content**
- [Installation](#installation)
- [Usage](#Usage)
- [Contributors](#contributors)
- [Features](#features)
- [License](#license)

## Installation
**1. Quick Installation**   
> :warning: **You must first reference the package AV in the web page**  
> `<script src="//cdn1.lncld.net/static/js/3.0.4/av-min.js"></script>`
```html
<script src="./dist/Valine.min.js"></script>
```
**2. Get `App ID`/`App Key` from LeanCloud**  
[Click here](https://leancloud.cn/dashboard/login.html#/signup) to register or login in `LeanCloud`.  
[Click here](https://leancloud.cn/dashboard/applist.html#/newapp) Create new application in `LeanCloud`, and you will get `appId`/`appKey`.

**3. Transfer Your Data**

[Disqus2LeanCloud](https://github.com/DesertsP/disqus2valine)

**4. Administration**

[Valine Admin](https://github.com/DesertsP/Valine-Admin)

## Usage
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Valine - A simple comment system based on Leancloud.</title>
    <script src="//cdn1.lncld.net/static/js/3.0.4/av-min.js"></script>
    <script src="./dist/Valine.min.js"></script>
</head>
<body>
    <div class="comment"></div>
    <script>
      new Valine({
          el: '#disqus_thread',
          smiles_url: '/smiles',
          app_id: 'Your App ID',
          app_key: 'Your Key',
          placeholder: '老司机来一发吧 O(∩_∩)O~~'
      });
    </script>
</body>
</html>
```
## Contributors
- [Contributors](https://github.com/panjunwen/Valine/graphs/contributors)

## Features
- Support for full markdown syntax
- Syntax highlighting
- And more...

## License

[GPL-2.0](https://github.com/xCss/Valine/blob/master/LICENSE)