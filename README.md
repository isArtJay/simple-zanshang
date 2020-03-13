# 赞赏功能实现
点击赞赏按钮，就会出现一个赞赏弹窗，简单的使用了几张二维码图片替换，所以没法显示有哪些人打赏

[在线Demo](<https://www.lien.run/Demo/reward/>)

# 效果预览:

![](https://artjay-1258580758.cos.ap-shanghai.myqcloud.com/7_enioyme/xiaoguo.gif)

# 用法示例

直接 clone 这个项目，把 css、HTML、js 代码分别放到相应的位置就可以了

# 须知

二维码图片是放在当前目录中的 images 文件中，支付宝和微信的命名规则为：`type+'-'+data-num`

- 如果选择2元，同时选择支付宝付款方式时，则对应的图片就是`alipay-2.png`

  ```html
  <button class="btn btn-blink" data-num="2">2元</button>
  ```

- 如果选择10元，同时选择微信付款方式时，则对应的图片就是`wechat-10.png`

  ```html
  <button class="btn btn-blink" data-num="10">10元</button>
  ```


**记得替换images路径下的二维码为你自己的，不然别人打款就会打给我的啦~**
