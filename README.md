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


> 4. SVG basic shape drawing

```html
rect属性：( 矩形 )

	basic -> ( x,y,width,height )
	rx ->  x轴圆弧半径
	ry ->  y轴圆弧半径

circle属性：( 圆 )

	basic -> ( cx,cy,r,[默认黑色填充，没有轮廓线])

ellipse属性：( 椭圆 )

	basic -> ( cx,cy,rx,ry )

polygon属性：( 多边形 [自动封闭] )

	basic -> points
	points -> 多边形的顶点坐标 ( 按照逗号或者空格隔开 两个一组 ) 例子：points=" 15,10 55,10 45,20 5,20 "

polyline属性： ( 多条线段 [不自动封闭] )

	basic -> points
	points -> 不规则线段的顶点坐标 例子: points='30 30, 45 15, 60 30'
		
stroke规则：( 描边 )

	stroke -> 颜色值：red|#f00|rgb(255,0,0)|rgb(60%,20%,60%)|rgba(255,0,0,1)|transparent
	stroke-width -> 线条的宽度( number )
	stroke-opacity -> 线条的不透明度( 0.0 ~ 1.0 )
	stroke-dasharray -> 线条的形态( 点线 | 虚线 ) stroke-dasharray = ' 长度 , 间隙 ' style='stroke-dasharray = 长度,间隙' ( 偶数个数字，如果是奇数个会重复执行一遍 )
	stroke-linecap -> 指定不同的值来确定线的头尾形状 值：[ butt (default) | round | square ] 默认butt精确与起止位置对其, round和square在起止位置都超过了真实位置	
	stroke-linejoin -> 主要用于polyline, 指定线段在拐角处交叉时的效果 值：[ miter (尖的) | round(圆的) | bevel(平的) ]


fill规则: ( 填充 )

	fill -> 颜色值
	fill-opacity -> 形状填充透明度 ( 0.0 ~ 1.0 )
	fill-rule ->  nonzero[默认值] | evenodd [填充外部图形] 
```

> 更多内容请详见 [小青蛙的博客](http://blog.sina.com.cn/riversfrog "小青蛙的博客") 谢谢！
