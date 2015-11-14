# Tolearn-List

## [Babel](https://babeljs.io/ "进入官网")
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

> 这个工具的配置文件是`.babelrc`，可以配置插件列表和其他信息。比如
> 
    {
      "plugins": ["transform-react-jsx"],
      "ignore": [
        "foo.js",
        "bar/**/*.js"
      ]
    }
> 


## [Bower](http://bower.io/ "进入官网")
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



## [webpack](https://webpack.github.io/)


## [node](https://nodejs.org/en/)


## [react]()


## [react-native]()
