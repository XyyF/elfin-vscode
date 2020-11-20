# diffVSCode
vscode for elfin

#### 本地打包
个人应用扩展，暂未发布应用市场

```js
npm i vsce -g

vsce package
```
从扩展的右上角选择Install from VSIX安装

### 功能列表

- [teenager] 文件适配wekf改造，适用于快速初始化Page.js文件

> 优势：专注于Page.js文件中，避免到处Copy文件内容，再删除逻辑的繁琐过程

1. Page文件中的 .js 文件
2. App文件中的 app.js 文件
<br/>
 <img src="https://rengar-1253859411.cos.ap-chengdu.myqcloud.com/img/20201113_112531.gif" width = "500" height = "500" alt="图片名称" style="margin: 0 auto;display: block;" />
<br/>

- [wekf] 属性补全提示

> 优势：对于新同学熟悉上手wekf十分友好，在不确定某些属性方法是否存在是也可以快速定位，让注意力专注于业务中，免去切换工程反复查找的过程

<br/>
 <img src="https://rengar-1253859411.cos.ap-chengdu.myqcloud.com/img/20201113_112858.gif" width = "600" height = "400" alt="图片名称" style="margin: 0 auto;display: block;" />
<br/>

- [wekf] 属性跳转定义文件

> 优势：结合wekf的属性补全，可以快速查看wekf属性实现逻辑，让注意力专注于业务中，免去切换工程反复查找的过程

<br/>
 <img src="https://rengar-1253859411.cos.ap-chengdu.myqcloud.com/img/20201113_113227.gif" width = "600" height = "300" alt="图片名称" style="margin: 0 auto;display: block;" />
<br/>

- [小程序] navigation路径跳转，支持 .js、.wxml、.json 文件

> 优势：某些时候想快速跳转到相应的文件 || 不太确实路径是否正确，可以免去在资源管理器中一步步对照文件路径的过程
> 特别是在 navigation方法、app.json文件路径、project.config.json预览路径

```js
// 支持以下格式跳转
"/pages/index/demo"
"/pages/index/demo?query=" + 1
'/pages/index/demo'
'/pages/index/demo?query=' + 1
`/pages/index/demo`
`/pages/index/demo?query=${xxx}`
// 可以不再前面加 /
"pages/index/demo"
// 可以支持自定义文件后缀 .wxml、.json、.wxss，默认为.js
"pages/index/demo.wxml"
...
```
<br/>
 <img src="https://rengar-1253859411.cos.ap-chengdu.myqcloud.com/img/20201110_094616.gif" width = "600" height = "400" alt="图片名称" style="margin: 0 auto;display: block;" />
<br/>

- [小程序] 新建小程序Page、Component文件

> base on 微信开发者工具功能，快速新建Page、Component，新建的Page还会在app.json/pages中添加路径，并在其基础上进行扩展
> 优势：文件名格式支持: test、test/test2，允许在指定附带文件夹名称

<br/>
 <img src="https://rengar-1253859411.cos.ap-chengdu.myqcloud.com/img/20201113_113535.gif" width = "600" height = "400" alt="图片名称" style="margin: 0 auto;display: block;" />
<br/>

- [小程序] 添加当前页面编译条件至project.config.json

> 优势：快速的编译当前的Page，会自动修改 project.config.json 中的Page编辑内容，免去在json文件反复查找、添加编译条件 && 减少文件体积，减小冲突的可能性
> 优势2：支持预置 query列表，提供选择 || 自定义，快捷针对不同场景进行调试

<br/>
 <img src="https://rengar-1253859411.cos.ap-chengdu.myqcloud.com/img/20201120_120411.gif" width = "1000" height = "500" alt="图片名称" style="margin: 0 auto;display: block;" />
<br/>

- [teenager] 对比远端最新的UI文件内容

> 优势：当远端UI文件发生了变动，本地快速对比内容，进行修改，免去两个工程反复比较文件内容


<br/>
 <img src="https://rengar-1253859411.cos.ap-chengdu.myqcloud.com/img/20201120_120645.gif" width = "700" height = "500" alt="图片名称" style="margin: 0 auto;display: block;" />
<br/>