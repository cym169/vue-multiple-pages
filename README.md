# vue多页面应用模板

**Vue PC端多页面应用模板 ，基于Vue 2, Webpack4, Element-UI**
**也集成了sass，less。初始化的时候可以进择**

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

访问 [http://localhost:8010/user/login.html](http://localhost:8010/user/login.html)

访问 [http://localhost:8010/user/index.html](http://localhost:8010/user/index.html)

访问 [http://localhost:8010/customer/index.html](http://localhost:8010/customer/index.html)

#### 打包

```bash
$ npm run build
$ node server.js #listen 2333 port
```

访问 [http://localhost:2333/user/login.html](http://localhost:2333/user/login.html)

访问 [http://localhost:2333/user/index.html](http://localhost:2333/user/index.html)

访问 [http://localhost:2333/customer/index.html](http://localhost:2333/customer/index.html)


## 项目结构

```bash
.
├── README.md
├── build // webpack config
│   ├── webpack.base.conf.js
│   ├── webpack.dev.conf.js
│   └── webpack.prod.conf.js
├── dist // dist
│   ├── assets
│   │   ├── css
│   │   │   ├── commons.css
│   │   │   ├── commons.css.map
│   │   │   ├── customer
│   │   │   │   ├── home.css
│   │   │   │   ├── home.css.map
│   │   │   │   ├── home2.css
│   │   │   │   └── home2.css.map
│   │   │   └── user
│   │   │       ├── index.css
│   │   │       ├── index.css.map
│   │   │       ├── login.css
│   │   │       └── login.css.map
│   │   ├── img
│   │   │   └── element-icons.6f0a763.ttf
│   │   └── js
│   │       ├── commons.js
│   │       ├── commons.js.map
│   │       ├── customer
│   │       │   ├── home.js
│   │       │   ├── home.js.map
│   │       │   ├── home2.js
│   │       │   └── home2.js.map
│   │       └── user
│   │           ├── index.js
│   │           ├── index.js.map
│   │           ├── login.js
│   │           └── login.js.map
│   ├── customer
│   │   ├── home.html
│   │   └── home2.html
│   ├── logo.png
│   └── user
│       ├── index.html
│       └── login.html
├── package.json
├── postcss.config.js
├── server.js
└── src
    ├── assets
    │   ├── css
    │   └── img
    │       └── logo.png
    ├── components
    │   └── modal.vue
    └── pages
        ├── customer
        │   ├── home
        │   │   ├── app.html
        │   │   ├── app.js
        │   │   └── app.vue
        │   └── home2
        │       ├── app.html
        │       ├── app.js
        │       └── app.vue
        └── user
            ├── index
            │   ├── app.html
            │   ├── app.js
            │   └── app.vue
            └── login
                ├── app.html
                ├── app.js
                └── app.vue
```

## 注意

**若需修改结构，记得在webpack.base.conf.js文件中修改相对应的路径，这个是需要注意的。**

**server.js是为了方便演示使用。若不需要可以删除。**

## License

MIT
