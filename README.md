![svg](/images/svg.png)

## svg exercises

> 1. Draw a cat with svg

* path , polyline, use的使用
* transform 形状的改变
* style, stroke, fill 的使用


> 2. Inline SVG in HTML

* viewBox的使用 
* viewBox = '最小X轴数值 最小y轴数值 宽度 高度'
* css控制svg形状颜色边框等

> 3. SVG House ViewBox

* 单位 : em ex px pt pc(12pt) cm mm in(英寸)
* preserveAspectRatio的使用
* preserveAspectRatio = "[xMinYMin|xMinYMid|xMidYMid|xMidYMin...] [meet|slice]"
* preserveAspectRatio = "none" (视口比例固定不会改变)
* 一般情况下，视口的改变需要preserveAspectRatio和viewBox的配合使用

```html
<svg width="4cm" height="5cm" viewBox="0 0 64 80" preserveAspectRatio = "none">//...</svg>

<svg width="1cm" height="5cm" viewBox="0 0 64 80" preserveAspectRatio = "none">//...</svg>
```
![svg](/images/preserveAspectRatio.png)


> 更多内容请详见 [小青蛙的博客](http://blog.sina.com.cn/riversfrog "小青蛙的博客") 谢谢！
