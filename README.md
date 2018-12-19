# travel

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


## 项目代码结构

README.md：项目说明文件
package.json：第三方依赖包
package-lock.json：锁文件，确定第三方依赖包的版本
index.html：默认首页模版
.postcssrc.js：postcss的配置项
.gitignore：指定格式文件不上传到git中
.eslintrc.js：代码规范检测
.eslintignore：指定文件夹下内容不受eslintrc.js检测
.editorconfig：配置编辑器语法
.babelrc：vue单文件解析器，转换浏览器可以解析的内容
static：静态资源
node_modules：第三方依赖的包
src：整个项目源代码
- assets：项目的图片
- components：项目的组件
- router：项目的路由
- App.vue：原始的根组件
- main.js：项目的入口文件
config：项目的配置文件
- index.js：基础的配置信息
- dev.env.js：开发环境的配置信息
- prod.env.js：线上环境的配置信息
build：项目打包的webpack的内容
