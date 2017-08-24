# css_components
css公共组件

## CSS常用组件使用说明

在HTML文档中输入相对应的HTML结构标签（包含class类名），并引入CSS文件即可：

```
<link rel="stylesheet" href="components.css">
```

- input输入框
`HTML`：
```
<input type="text" class="input-text-box" placeholder="文字">
```

- button
`单个button彩色按钮`：

```
HTML：
<button class="btn-set-color">Yes!</button>
更改按钮颜色只需用background-color:;来覆盖即可。
更改按钮大小：直接更改字体大小
单个或多个button（经典按钮）
默认样式
鼠标划上时效果
HTML：
<div class="btn-set-many">
    <button class="btn left">Left</button>
    <button class="btn middle">Middle</button>
    <button class="btn right">Right</button>
</div>
添加或删除按钮直接在HTML结构中更改标签的多少。
更改按钮大小直接更改字体大小。
更改按钮背景颜色：

复选框

HTML：
<input type="checkbox" id="watermelon" name="checkbox"/>
<label for="watermelon">西瓜</label>
<input type="checkbox" id="grape" name="checkbox"/>
<label for="grape">葡萄</label>
注意：一个input必须用id和一个label绑定.
更改复选框大小：更改其字体大小。
更改选中后复选框的颜色（颜色需要用rgba来写）：
.customize-checkbox:checked+label::before{
    content:'\2713';
    background: rgba(150, 197, 47, 0.49);
}
单选

HTML：
<input type="radio" id="radio" name="radio" class="radio"/>
<label for="radio">李易峰</label>
<input type="radio" id="bbb" name="radio" class="radio"/>
<label for="bbb">杨洋</label>
更改单选框的大小和选中的颜色同复选框相同。
下拉框
经典下拉框：

HTML:
<div class="dropdown">
    <div class="dropdown-toggle">
        dropdown
        <span class="caret"></span>
    </div>
    <ul class="dropdown-menu">
        <li><a href="#">Action</a></li>
        <li><a href="#">Action</a></li>
        <li><a href="#">Another action</a></li>
        <li><a href="#">Something else here</a></li>
        <li><a href="#">Separated link</a></li>
    </ul>
</div>
带分割线下拉框

只需在dropdown-menu中加：
<li class="dividing-line"></li>
HTML:
<div class="dropdown">
    <div class="dropdown-toggle">
        dropdown
        <span class="caret"></span>
    </div>
    <ul class="dropdown-menu">
        <li><a href="#">Action</a></li>
        <li><a href="#">Action</a></li>
        <li><a href="#">Another action</a></li>
        <li class="dividing-line"></li>
        <li><a href="#">Something else here</a></li>
        <li><a href="#">Separated link</a></li>
    </ul>
</div>
数量加减
数量加减（经典）：

HTML:
<div class="quantity-add-less-classic">
    <button class="less">-</button>
    <input type="text" class="quantity-input-num" value="1">
    <button class="add">+</button>
</div>
数量加减（分离)：

HTML:
<div class="quantity-add-less-Separation">
    <input type="text" class="quantity-input-num" value="1">
    <div class="add-less">
        <button class="add">+</button>
        <button class="less">-</button>
    </div>
</div>
数量加减(分割)：

HTML:
<div class="quantity-add-less-Separation quantity-add-less-spacing">
    <input type="text" class="quantity-input-num" value="1">
    <div class="add-less">
        <button class="add">+</button>
        <button class="less">-</button>
    </div>
</div>
```
