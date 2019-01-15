# scroll
自己造了一个上下翻页插件，不需要任何依赖

# 使用
```javascript
new iSlider({
        wrap:'.wrap',
        item:'.item',
        playClass:'play',
        onslide:function (index) {
            console.info(index)
        }
    });
```
# 参数
```
@param {string} opts.wrap='.wrap' 容器 
@param {string} opts.item='.item'  滚动单元的元素
@param {string} opts.playClass='play'  触发播放动画的class
@param {number} [opts.index=0]  设置初始显示的页码
@param {number} [opts.speed=400] 动画速度 单位:ms
@param {number} [opts.triggerDist=30] 触发滑动的手指移动最小位移 单位:像素
@param {boolean} [opts.isVertical=true] 是否是垂直滑动 默认是.  设成false为水平滑动
@param {boolean} [opts.useACC=true] 是否启用硬件加速 默认启用
@param {boolean} [opts.fullScr=true] 是否是全屏的 默认是. 如果是局部滑动,请设为false
@param {function} [opts.onslide]  滑动后回调函数  会回传index参数
```

# 需要改进
1. 处理图片加载
2. 记录上次页面位置
3. 优化
