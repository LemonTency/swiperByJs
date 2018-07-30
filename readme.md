
#####页面结构
原理（通过图片位置的变换来实现轮播，container位置有限，一次只能显示一张，container的宽度长度就是我们能看到的轮播图的长度宽度，如果哪站图片移动到那里的时候，就显示那一张）
问题一：
为什么要前面后面各多加一张照片
![image.png](https://upload-images.jianshu.io/upload_images/7728915-da6f6996ee578225.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
#####箭头切换
 定义click事件，定义animation(offest)
#####无限滚动
next点击时，若当前图片索引值为4(一共有4张要显示的图片）,则令index = 1；重新定位。prev点击时，若当前图片索引值为1,则令index = 4;
#####按钮切换
定位当前按钮索引值（getAttribute)，两个索引之差再进行计算。
#####定时播放
定时器。