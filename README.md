#drawing-board
#HTML5中canvas实现画板功能:除了绘画功能以外,还有改变线条颜色,粗细,清屏,撤销,橡皮擦等功能.
HTML部分
input type = color
input type = range

css部分
input type = range的自定义样式.消除默认样式,添加滑道样式,添加滑动点样式

js部分
1.绘画功能--->获取一个2d画布对象,监听鼠标mousedown和mousemove事件,记录鼠标按下时相对于画布原点的坐标.
2.拾色器--->获取拾色器的值,作为线条的颜色.
3.清屏功能--->点击清屏时,调用clearRect()方法,清楚画板大小的像素.
4.撤销功能--->绘画时,用一个数组存放每一笔绘画结束后的image.点击撤销时,把删除最后一位的数组通过putImageData()重新放入画布中.
5.橡皮擦--->将线条颜色换成画布背景色.
6.线条粗细--->获取range的值,作为线条粗细.
