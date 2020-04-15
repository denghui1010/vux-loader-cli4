# vux-loader-cli4

[![npm][npm]][npm-url]

### 说明

基于 [vux](https://github.com/airyland/vux) 的 [@vux/loader](https://www.npmjs.com/package/@vux/loader)@2.0.0-rc4 修改而来, 可以在 vue-cli@4.x 中正常工作

### 安装
```npm install vux-loader-cli4 --save-dev```


### 使用

vue.config.js

```Javascript
module.exports = {
    configureWebpack: (config) => {
        require("vux-loader-cli4").merge(config, {
            plugins: ["vux-ui"],
        });
    },
    transpileDependencies: [/vux/]
}
```

[npm]: https://img.shields.io/npm/v/vux-loader-cli4.svg
[npm-url]: https://www.npmjs.com/package/vux-loader-cli4
