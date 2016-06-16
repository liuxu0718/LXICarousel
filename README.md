# LXICarousel
本demo 只是对iCarousel原生demo中提供的动画进行了一个组合。最终并没有完全实现National Geographic Atlas里card的滑动。

# iCarousel 原始demo 

https://github.com/nicklockwood/iCarousel

## 卡片动画
主要是CATransform3D. 最终要实现理想动画需要自定义一个CATransform3D.

## 修改部分，添加了两个属性 新增一个方法

###属性 firstCardType
可以自定义第一个card的动画类型（由于目前写不出来完美的CATransform3D, 这里的类型依旧依赖原始的动画）。

###属性isGradually 
控制第一个card是否透明。

###方法 - (CATransform3D)newTransformForItemViewWithOffset:(CGFloat)offset 
为了不破坏原始代码的逻辑 新定义了一个方法。

## 详情代码里都有注释

##声明：此demo只是对iCarousel进行微调，不喜勿喷。有什么问题可以issue我。



![image](https://github.com/liuxu0718/LXICarousel/blob/master/LXICarousel.gif)

