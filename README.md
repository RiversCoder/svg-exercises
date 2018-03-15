![svg](/images/svg.png)

## svg demos

> 1. 进度球案例
* 水波纹滚动进度球案例 [Demo在线查看](https://riverscoder.github.io/svg-exercises/17_svg_progress_up.html 'Demo查看')

>2. 组合旋转特效案例
* Js动态创建组合旋转特效案例 [Demo在线查看](https://riverscoder.github.io/svg-exercises/14_svg_shape_animation.html 'Demo查看')

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


> 4. SVG Basic Shape

* rect属性：( 矩形 ) 
* circle属性：( 圆 ) 
* ellipse属性：( 椭圆 )
* polygon属性：( 多边形 [自动封闭] )
* polyline属性： ( 多条线段 [不自动封闭] )	
* stroke规则：( 描边 )
* fill规则: ( 填充 )


> 5. SVG Shape Style

* 内部样式表 : style标签内部
* 外部样式表 : link标签引入
* 表现属性 : 行内属性
* 优先级 : 内部 > 外部 > 表现

> 6. SVG Group and reference objects

* g use defs symbol image
* xlink:href='#Id'




> 更多内容请详见 [小青蛙的博客](http://blog.sina.com.cn/riversfrog "小青蛙的博客") 谢谢！
