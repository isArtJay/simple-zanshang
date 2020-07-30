# 博客赞赏插件
点击赞赏按钮，就会出现一个赞赏弹窗，使用收款码进行收款，所以没法显示有哪些人打赏。

[在线Demo](<https://www.lien.run/Project/reward/>)

# 效果预览

<img align="center" src="https://raw.githubusercontent.com/isArtJay/simple-zanshang/master/src/demo.gif"></img>

# 用法示例

直接 clone 这个项目，把 css、HTML、js 代码分别放到相应的位置：

HTML：

```html
<!-- 赞赏按钮 -->
<div class="entry-shang text-center">
  <button class="zs show-zs btn btn-bred">赞赏</button>
</div>
<!-- 全屏遮罩背景 -->
<div class="zs-modal-bg"></div>
<div class="zs-modal-box">
  <div class="zs-modal-head">
    <!-- 关闭按钮 -->
    <button type="button" class="close">×</button>
    <!-- 左上角logo和文字 -->
    <span class="author"> <img src="./images/logo.ico" />Lien </span>
    <p class="tip"><i></i><span>谢谢你的赞赏~</span></p>
  </div>
  <div class="zs-modal-body">
    <div class="zs-modal-btns">
      <button class="btn btn-blink" data-num="2">2元</button>
      <button class="btn btn-blink" data-num="5">5元</button>
      <button class="btn btn-blink" data-num="10">10元</button>
      <button class="btn btn-blink" data-num="50">50元</button>
      <button class="btn btn-blink" data-num="100">100元</button>
      <button class="btn btn-blink" data-num="1">任意金额</button>
    </div>
    <div class="zs-modal-pay">
      <button class="btn btn-bred" id="pay-text">2元</button>
      <p>使用<span id="pay-type">微信</span>扫描二维码完成支付</p>
      <img src="./images/wechat-btn.png" id="pay-image" />
    </div>
  </div>
  <div class="zs-modal-footer">
    <!-- 支付宝控件 -->
    <label>
      <input
        type="radio"
        name="zs-type"
        value="alipay"
        class="zs-type"
        checked="checked"
      />
      <span class="zs-alipay"><img src="./images/alipay-btn.png"/></span>
    </label>
    <!-- 微信控件 -->
    <label>
      <input type="radio" name="zs-type" value="wechat" class="zs-type" />
      <span class="zs-wechat"><img src="./images/wechat-btn.png"/></span>
    </label>
    <!-- 清除浮动 -->
    <div class="clear"></div>
  </div>
</div>
```

CSS：

```html
<link rel="stylesheet" href="reward.css" />
```

JS：

```html
<script src="jquery.min.js"></script>
<script src="reward.js"></script>
```

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