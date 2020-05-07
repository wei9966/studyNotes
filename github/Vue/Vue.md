## Vue

### 官网教程

1. 安装npm  安装node.js

2. 安装cnpm

   npm install -g cnpm --registry=https://registry.npm.taobao.org

3. 安装vue-cli

   cnpm install -g @vue/cli

4. 安装webpack

   > cnpm install -g webpack

5. 初始化创建项目

   > vue ui

### webpack创建项目

1. vue init webpack 项目名即可

### VUE-CLI

#### 项目目录

1. config

   > config配置文件
   >
   > index.js 中可以修改端口号
   >
   > autoOpenBrowser: true 打开浏览器

2. build

   > 构建项目

3. src 目录文件

4. static 静态资源文件

5. .babelrc runtime controller bable配置文件

6. eslintrc  eslint配置

7. eslintignore 忽略文件

8. gitignore git忽略

9. index.html 页面

10. package.json 依赖

#### 运行

> npm run dev

#### main.js 入口文件

#### 全局配置axios

```js
axios.defaults.baseURL='';//配置前置路径
axios.defaults.headers.common['Authorization']='token'
axios.defaults.headers.post['Content-type']='application/json'
axios.defaults.headers.get['Accepts']='application/json'


```

#### 全局配置文件axios

```js
import axios from 'axios'
const instance=axios.create({
    baseURL:''
}
)
instance.defaults.hreaders.common
export default instance//导出
```

