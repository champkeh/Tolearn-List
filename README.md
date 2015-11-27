# Tolearn-List



## [Babel](https://babeljs.io/ "进入官网查看详细的使用文档")
这是一款JavaScript的编译器(代码转换器)，主要用于转换JavaScript代码。比如，把ES2015(ES6+)的代码转换为ES5的代码，或者把JSX的代码转换为常规的JavaScript代码(Babel对React的支持非常好)

> 需要注意的是，6.0.0之前的版本可以直接转换代码，6.0.0这个版本进行了重构，仅仅安装babel-cli或者babel-core并不能转换代码，你需要**安装插件**。每一个ES6+的新特性都对应一个插件，同时官方也提供了一些常用的preset，直接使用这些preset可以避免自己手动配置插件列表。

关于6.0.0的版本重构，可参考官方博客的文章：[6.0.0 Released](http://babeljs.io/blog/2015/10/29/6.0.0/)

插件列表：[plugins](http://babeljs.io/docs/plugins/)

#### Example
1. 命令行下使用babel进行代码转换
```bash
$ npm install -g babel-cli              # 安装命令行工具
$ npm install babel-preset-es2015       # 安装es2015 preset
$ babel example.es6 --presets es2015 -o example.js       # 代码转换
```

> 这个工具的配置文件是`.babelrc`，可以配置插件列表和其他信息(可用配置项在[这里](http://babeljs.io/docs/usage/options/))。比如
> 
    {
      "presets": ["es2015"],
      "ignore": [
        "foo.js",
        "bar/**/*.js"
      ]
    }
> 



## [Bower](http://bower.io/ "进入官网查看详细的使用文档")
Bower是一个包管理工具，主要用于web前端。作用和node里面的npm，asp.net里面的NuGet等类似。管理网站中用到的框架，库，资源文件等等

Bower最大的特点就是**flat dependency tree**，每个包只需要一个版本，非常适合于前端。

> 注意：Bower本身是一个命令行工具，这个工具的配置文件是`.bowerrc`，这个文件的详细配置请参考[bower/spec](https://github.com/bower/spec/blob/master/config.md)
> 
> 而使用Bower管理的包也有一个配置文件(或者叫包的**定义文件**)，叫`bower.json`，关于这个文件的配置请参考[bower/spec](https://github.com/bower/spec/blob/master/json.md)
> 
> 这两个文件都使用JSON格式进行配置的

经Bower管理起来的包，你可以直接使用。比如：
```html
<!-- 直接在网站中使用Bower安装过的包 -->
<script src="bower_components/jquery/dist/jquery.min.js"></script>
```
但是官方推荐我们配合其他一些工具来使用Bower，参考[这篇文章](http://bower.io/docs/tools/)



## [webpack](https://webpack.github.io/ "进入官网查看详细的使用文档")
这是一个模块打包工具，非常强大，也相对复杂了些，比较一下官方文档就知道了(这个工具的文档是上面那两个工具文档之和)。
关于这个打包工具的作用，用官方的一幅图来说明最合适不过了：
![what-is-webpack.png](https://webpack.github.io/assets/what-is-webpack.png)

把模块经过这样的打包处理之后，可以达到下面这些目的：
- 把依赖树分割成小块，以便能够按需加载
- 保持初始加载时间仍然很小
- 每一个静态资源文件都可以成为一个模块
- 适合于SPA和大项目

### 学习资源
- [SurviveJS - Webpack and React](http://survivejs.com/)一本不错的书



## [node](https://nodejs.org/en/ "进入官网查看详细的使用文档")



## [react](http://facebook.github.io/react/ "进入官网")
### 学习资源
- [谈谈React.js的核心入门知识](http://web.jobbole.com/83414/ "伯乐在线")
- [源码剖析系列](http://zhuanlan.zhihu.com/purerender "pure render - 知乎专栏")
- [ReactJS Example](http://react.rocks/) (这个网站有最新的 ReactJS 组件示例，是学习 React 的好东西)



## [react-native](https://facebook.github.io/react-native/ "进入官网")
### 学习资源
- [深入浅出 React Native: 使用 JavaScript 构建原生应用](http://zhuanlan.zhihu.com/FrontendMagazine/19996445 "知乎专栏")
- [React Native 通信机制详解](http://blog.cnbang.net/tech/2698/)
- [React Native 之布局篇](http://segmentfault.com/a/1190000002658374)
- [React Native 组件库](https://react.parts/native)
- [11款开源组件](http://www.oschina.net/news/61214/11-react-native-ui-components)

> 最后，附上Github上别人整理的学习资源:
> [React-Native 学习指南](https://github.com/ele828/react-native-guide)



## [Redux](http://rackt.org/redux/ "进入官网")
这是一个为JavaScript App准备的可预测的状态容器，可以和任何一款View Library(包括React)搭配使用。



> 最后附上一些大牛的博客地址
> 
> 1. [http://blog.vjeux.com/](http://blog.vjeux.com/) Facebook 前端团队的软件工程师，负责 React Native 项目

