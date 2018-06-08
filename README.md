# vue多页面应用模板

**Vue PC端多页面应用模板 ，基于Vue 2, Webpack4, Element-UI**

## 依赖

1. [Vue2](https://github.com/vuejs/vue)
2. [Webpack4](https://github.com/webpack/webpack)
3. [ElementUI](https://github.com/ElemeFE/element)
4. [Postcss](https://github.com/postcss/postcss)([autoprefixer](https://github.com/postcss/autoprefixer) default)
5. [Less](http://lesscss.org/)
6. [Sass](https://github.com/webpack-contrib/sass-loader)

## 开始

#### 初始化项目

``` bash
$ npm install -g vue-cli
$ vue init cym169/vue-multiple-pages new-project
$ cd new-project
$ npm install
```

#### 测试

```bash
# serve with hot reload at localhost:8010
$ npm run dev
```

访问 http://localhost:8010/login.html

访问 http://localhost:8010/index.html

#### 打包

```bash
$ npm run build
$ node server.js
```

访问 http://localhost:2030/index.html

## 注意

```bash
若需修改结构，记得在webpack.base.conf.js文件中修改相对应的路径，这个是需要注意的
若不需要Element-UI或者其他插件，请自行修改
autoprefixer已经挂在postcss.config.js中了，请自行根据它的API来配置
```

## License

MIT
