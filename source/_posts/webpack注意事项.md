---
title: webpack注意事项
date: 2021-02-18 13:31:29
tags:
	- webpack
	- webpack-cli
categories: webpack
---



## html-webpack-plugin 报错 

### Error: The loader didn't return html

报错原因：[Webpack v5.22.0`破坏了HTMLWebpackLoader ](https://github.com/jantimon/html-webpack-plugin/issues/1603)

解决方案： package.json 中 html-webpack-plugin 版本号是`"^4.5.0"`  直接更新至`5.1.0`

### Error: Automatic publicPath is not supported in this browser

设置 webpack.config.js 中 output 中 publicPath: ''  为空字符串