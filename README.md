# Ant-Design-Pro
Ant Design Pro网页布局练习（flex、grid、响应式布局）

## 笔记

1. 父元素选择器 子元素选择器:nth-child(n)
2. 属性选择器：[class*='name']
3. background-size:
    - contain：保持比例，图片全部展示出来
    - cover：保持比例，图片全部铺满容器
4. 
CSS定义变量：
```css
:root{
    --变量名：属性值;
}
```
使用：
```css
var(变量名)
```
JS代码获取或修改CSS中的变量：
```javascript
元素对象.style.getPropertyValue(变量名);
元素对象.style.setProperty(变量名,变量值);
//CSS变量一般定义在根元素（html）上，这样便可全局获取到了
//所以上面的元素对象一般都是document.documentElement
```
5. CSS布局元素名字的规则：
    - g-xxx：表示通用布局
    - m-xxx：表示通用模块（可重复使用的较大整体）
    - u-xxx：表示通用元件（不可再分的个体，可重复在各种模块中使用）
    - j-xxx：仅供js使用的
6. 固定定位元素是脱离文档流的，即使它在弹性盒子内
7. 固定定位的元素的宽度是由其内容决定，若需保证其宽度和元素的一样，可使用```width:inherit;```。**但是**，若父元素没有给定宽度（比如是弹性布局中的盒子），此时使用inherit是不生效的。可设置成100%，再使用层级z-index控制和其他元素得关系
8. not伪类：表示没有包含指定选择器时生效
```css
选择器:not(选择器1,...,选择器n)
```
9. is伪类：表示包含指定选择器时生效
```css
选择器:is(选择器1,...,选择器n)
```
