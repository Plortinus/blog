#H5项目CSS总结(2015.12 ~ 2017.10)

1. 图片水平居中
```html
<div class="rinoa">
  &nbsp;<img src="./face.png" /> // 填充&nbsp;
</div>
```
```css
.rinoa {
  text-align: center; // 文字居中
}
```
2. 块级元素水平居中
```html
<div>
  <div class="center"></div>
</div>
```
```css
.center {
  width: 8rem;  // 设置宽度
  margin: 0 auto;  // 设置margin,左右auto,平分剩余空间
}
```
3. input或div中文字垂直居中
```html
<input class="center" type="text" />
<div class="center">你好,婉转喵!</div>
```
```css
.center {
  height: 100px;  // 高和行高相等
  line-height: 100px;
}
```
4. 元素垂直居中
```html
<div class="parent">
  <i class="iconfont"></i>
</div>
```
```css
.parent {
  position: relative; // 父元素设置非static的position属性
}
.iconfont {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);  //相对自身偏移
}
```