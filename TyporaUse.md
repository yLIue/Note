# Typora

## 更改字体代码模式的颜色

### 更改教程

1.shift + F12 打开开发者工具

2.利用定位工具去定位要改变的区域

3.在Styles中找到对应的区域

如:

```
base-cotrol.css:<line>
```

### 具体颜色

字体 `#AD4FD9`

光标 `#AD4FD9`

## base.user.css编写教程

### 文件创建

1.打开Typora-文件-偏好设置

2.选择外观-主题-打开主题文件夹

3.创建base.user.css文件(已有就编写)

### 编码格式声明

```css
@charset "<编码格式>";
```

### 更改字体

```css
body {
        font-family: '<字体名字>';
}
```

### 更改代码块字体

```css
.CodeMirror div.CodeMirror-code {
    font-family: '<字体名字>';
}
```

### 更改选中区域颜色

```css
::selection {
    background-color: #d3a4eb;
}
```

### 更改强调字体样式

```css
strong {
    color: #db3f1e;
}
```

### 更改标签样式

```css
h2 {
    color: #b85ce5;
}
```

### 更改高亮样式

```css
makr {
    background-color: #db91ff;
}
```

