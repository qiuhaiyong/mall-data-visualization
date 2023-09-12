# 1. 数据可视化

## 1.2 什么是数据可视化？

能够将数据以更加直观的形式展现。 --->图表

我们来看一组数据：

```
衬衫:5
羊毛衫:20
雪纺衫:36
裤子:10
高跟鞋:10
袜子:20
```

这个数据就是某些产品的销量. 单纯从这些文字上来看, 很难看出数据之间对比的关系. 如果把这些数据以图表的方式呈现出来呢 ?

![image-20230912202442378](C:\Users\yukiha\AppData\Roaming\Typora\typora-user-images\image-20230912202442378.png)

上面这幅图就是这组数据的图表展示. 通过这幅图一眼就能看出哪些产品销量高, 哪些产品销量低. 数据与数据之间的关系一目了然。

## 1.2 数据可视化的好处

- 清晰有效地传达与沟通信息

数据可视化的好处之一就是能够清晰有效的传达信息和沟通信息. 继续看刚才的那个例子, 如果使用同样的数据, 换成另外一种展现形式, 比如下边的这幅饼图. 我们可以很容易的就看出每个产品的销量占比.不需要太多的脑力计算和思维转换.

![image-20230912202621339](C:\Users\yukiha\AppData\Roaming\Typora\typora-user-images\image-20230912202621339.png)

- 更容易洞察隐藏在数据中的信息

将数据以图表的方式呈现出来还可以帮助我们感受到那些隐藏在数据之间的信息.比如下面的这幅上证指数的k线图

![image-20230912202657178](C:\Users\yukiha\AppData\Roaming\Typora\typora-user-images\image-20230912202657178.png)

# 2. Echarts

## 2.1 Echarts的基本使用

```
1：引入ecahrts.js文件
2：准备一个呈现图表的盒子
3：初始化echarts实例对象
4：准备配置项
5：将配置项设置给echarts实例对象
```

## 2.2 相关配置

- xAxis:直角坐标系中的x轴
- yAxis:直角坐标系中的y轴
- series:系列列表。每个系列通过type决定自己的图标类型

# 3. Echarts常用图表

```
1.柱状图
2.折线图
3.散点图
4.饼图
5.地图
6.雷达图
7.仪表盘图
```

## 3.1柱状图

特点：柱状图描述的是分类数据，呈现的是每一个分类中有多少，通过柱状图，可以很清晰的看出每个分类的排名情况。

### 3.1.1 常见效果

- 标记：最大值 最小值（markPoint） 平均值(markLine)
- x显示：数值显示(label) 柱宽度(barWidth) 横向柱状图(更改x轴和y轴的角色)

### 3.1.2 常见通用配置有哪些？

​	通用配置指的就是任何图标都能使用的配置

- title 标题
- tooltip 提示
- toolbox 工具按钮
- legend 图例

### 3.1.3 通用配置 title

- 文字样式： textStyle

- 标题边框：borderWidth
- 标题位置

### 3.1.4 通用配置tooltip

tooltil：提示框组件，用于配置鼠标滑过或点击图标时的显示框

- 触发类型：trigger

item、axis

- 触发时机：triggerOn

mousemove、click

- 格式化：formatter

字符串、回调函数

### 3.1.5 通用配置toolbox

Echarts提供的工具栏，工具栏。内置有[导出图片](https://echarts.apache.org/zh/option.html#toolbox.feature.saveAsImage)，[数据视图](https://echarts.apache.org/zh/option.html#toolbox.feature.dataView)，[动态类型切换](https://echarts.apache.org/zh/option.html#toolbox.feature.magicType)，[数据区域缩放](https://echarts.apache.org/zh/option.html#toolbox.feature.dataZoom)，[重置](https://echarts.apache.org/zh/option.html#toolbox.feature.reset)五个工具。

