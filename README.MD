# plus-draggable-element

一个可拖拽的html元素，可以把任何内容放入，变为一个可拖拽的组件，可以是一个div、文本，也可以是任何网页组件，自由拖动，在靠近屏幕边缘时，会自动隐藏为一个小浮标，浮标的内容可以自定义任何图片表示当前组件的类型，没有则提供默认浮标，点击浮标即可再次显示原组件内容

## How to use it?

```
npm install plus-draggable-element
```

### How to use it in the project!

```
import DraggableComponent from 'plus-draggable-element';

<div class="plus-draggable-component">
</div>

//全部参数
{
    initialPosition: "left", // 初始位置：center, top-left, top-right, bottom-left, bottom-right, left, right
    edgeFolding: true, // 是否允许边缘折叠，这里的折叠实际上是把容器隐藏，只显示出一个悬浮的按钮或其他的元素
    collapseDelay: 5000, //边缘折叠延迟时间，意思在一定时间后才折叠
    content: "", // 内容，可以是字符串或 HTML 元素
    buoyContainerWidth: 30, // 悬浮标记指示容器长度
    buoyContainerHeight: 30, // 悬浮标记指示容器高度
    buoyContent: null, // 悬浮标记指示内容，可以是 HTML 字符串、DOM 元素或图片 URL
    resizable: false, // 是否允许调整大小 (暂未实现)
}

//初始化拖拽组件，在页面加载完成后使用
new DraggableComponent({
    initialPosition: "right", // 初始位置为右边
    buoyContent: '', // 设置箭头内容为svg图标或者img
    content: "<h1>Hello, world!</h1>", // 设置组件内容，如果在网页中已经写有了class="plus-draggable-component"的标签，这里就自动无效
});
...
```
## 🖥 浏览器兼容性

- 现代浏览器

| [![edge](https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png)](http://godban.github.io/browsers-support-badges/) | [![Edge](https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png)](http://godban.github.io/browsers-support-badges/) | [![chrome](https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png)](http://godban.github.io/browsers-support-badges/) | [![safari](https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png)](http://godban.github.io/browsers-support-badges/) |
| ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Edge                                                                                                                                              | last 2 versions                                                                                                                                         | last 2 versions                                                                                                                                         | last 2 versions                                                                                                                                         |
  

### npm Docs

#### Documentation for the npm registry, website, and command-line interface

See [npm Docs](https://docs.npmjs.com/).
