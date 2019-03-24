# 赞赏功能实现
## 功能简介：

[更多详细介绍](<https://www.artjay.me/2019/enjoy-me/>)

点击赞赏按钮，就会出现一个赞赏弹窗，简单的使用了几张二维码图片替换，所以没法显示有哪些人打赏

## 效果预览:

目前我只开了微信赞赏，你可以自己设置支付宝和微信同时开

![](https://artjay-1258580758.cos.ap-shanghai.myqcloud.com/7_enioyme/xiaoguo.gif)

## 使用

直接clone这个项目，把css、HTML、js代码分别放到相应的位置就可以了

## 须知:

二维码图片是放在当前目录中的 images 文件中，支付宝和微信的命名规则为：`type+'-'+data-num`

- 如果选择2元，同时选择支付宝付款方式时，则对应的图片就是`alipay-2.png`

  ```html
  <button class="btn btn-blink" data-num="2">2元</button>
  ```

  ![img](https://artjay-1258580758.cos.ap-shanghai.myqcloud.com/7_enioyme/alipay.gif)

- 如果选择10元，同时选择微信付款方式时，则对应的图片就是`wechat-10.png`

  ```html
  <button class="btn btn-blink" data-num="10">10元</button>
  ```

  ![img](https://artjay-1258580758.cos.ap-shanghai.myqcloud.com/7_enioyme/wechat.gif)

**记得替换images路径下的二维码为你自己的，不然别人打款就会打给我的啦~**