# vue.js
###所有命令在git工具中输入(以下命令安装了git, node, vue.js)
###苏铭开发项目使用了node, git, vue.js, muse ui

#清除配置
`php artisan config:clear`
#清除缓存
`php artisan cache:clear`
#vue创建目录文件夹
`vue init webpack vue_3`

` cd vue_3`

`cnpm install`
#vue在目录中加载组件
`cnpm install --save muse-ui`

#打包vue项目命令
`cnpm run build`

#子div加浮动之后，父div撑不开问题
`display: inline-block;`

#vue下载主题组件
`cnpm install raw-loader --save`

#vue下载跨域组件
`cnpm install axios --save`

#vue下载轮播图组件
`/*老版本vue-touch不兼容2.0，会报错 Cannot read property 'priority' of undefined，请使用vue-touch@next版本*/Vue.use(VueTouch, {name: 'v-touch'})`
`cnpm install vue-touch@text --save `
`cnpm install vue-awesome-swiper --save `
#vue下载轮播图index.js中引用
`import VueAwesomeSwiper from 'vue-awesome-swiper'`
#vue下载轮播图index.js中使用
`if (process.browser) {const VueAwesomeSwiper = require('vue-awesome-swiper/ssr')Vue.use(VueAwesomeSwiper)}`

#muse ui自适应（index.html）
`<meta name="viewport" content="width=device-width, initial-scale=1.0">`
`<meta http-equiv="X-UA-Compatible" content="ie=edge">`

#C:\Windows\System32\drivers\etc

#vue城市及联
`第一步:webpack.base.conf.js页面中加入(1)var webpack = require("webpack")`
`(2)plugins: [
    new webpack.optimize.CommonsChunkPlugin('common.js'),
    new webpack.ProvidePlugin({
     jQuery: "jquery",
     $: "jquery"
    })
  ],`
  `(3)注释掉
  // {
  //   test: /\.(js|vue)$/,
  //   loader: 'eslint-loader',
  //   enforce: 'pre',
  //   include: [resolve('src'), resolve('test')],
  //   options: {
  //     formatter: require('eslint-friendly-formatter')
  //   }
  // },`
  `第二步:index.js页面中加入(1)import $ from 'jquery'  (2)Vue.use($)`
 `第三步页面中可以使用jquery语句`

