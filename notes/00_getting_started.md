# Vue重写JS30 - 起步

## 介绍

几个月前，我学过了Wes Bos写的[Javascript30](https://javascript30.com/)(比较惭愧，现在还没写完)。我从中学到了很多东西，今天刚好看到Dave Follett 要用vue重写JS30。我很高兴，因为我应该可以从他的vue30中学到很多东西。这里是他的[Getting Started文章](https://davefollett.io/2018/08/01/a-new-vue-on-javascript30-getting-started/)，之后的一系列文章会作为我的笔记记录或部分翻译他的文章，侵权必删。

## 引入Vue



```html
<head>
  <meta charset="UTF-8">
  <title>GETTING STARTED</title>
  <script src="https://cdn.bootcss.com/vue/2.5.16/vue.min.js"></script>
</head>
```

从[bootcdn](https://www.bootcdn.cn/vue/)中引入最新版的vue，当然你也可以遵循[Vue文档](https://cn.vuejs.org/v2/guide/installation.html)。

## 挂载DOM元素

```html
<div id="app">
   {{message}}
</div>
```

##  Vue 实例

```javascript
var app = new Vue({
  el: '#app',
  data: {
    message: "Hello World!"
  },
  computed: {
  },
  methods: {
  },
  mounted: function () {
  },
  watch: {
  }
})
```

下面是这些api的官方文档，这里先不去细说这些api的作用，等到之后用到的时候在解释。

* el - https://cn.vuejs.org/v2/api/#el
* data - https://cn.vuejs.org/v2/api/#data
* methods - https://cn.vuejs.org/v2/api/#methods
* mounted - https://cn.vuejs.org/v2/api/#mounted
* watch - https://cn.vuejs.org/v2/api/#watch 

## 组合在一起



```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>GETTING STARTED</title>
    <script src="https://cdn.bootcss.com/vue/2.5.16/vue.min.js"></script>
</head>

<body>
    <!-- 挂载DOM元素 -->
    <div id="app">
        {{message}}
    </div>
    <script>
        //  Vue 实例
        var app = new Vue({
            el: '#app',
            data: {
                message: "Hello Wolrd!"
            },
            computed: {

            },
            methods: {

            },
            mounted: function () {

            },
            watch: {

            }
        })
    </script>
</body>

</html>
```

## Credit

再次感谢Wes Bos的 [Javascript30](https://javascript30.com/) 和 Dave Follettt 的 [vue30](https://davefollett.io/2018/08/01/a-new-vue-on-javascript30-getting-started/), 侵权必删.

