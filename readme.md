[Improving Perceived Performance with Multiple Background Images](http://csswizardry.com/2016/10/improving-perceived-performance-with-multiple-background-images/)

# 加载图片空白处理
利用[Using CSS multiple backgrounds](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Background_and_Borders/Using_CSS_multiple_backgrounds)
步骤:
- 使用PS获取模糊颜色
  - 打开图片
    ![4.png](https://ooo.0o0.ooo/2016/11/12/5826890e2be8a.png)
  - 将图片分区
  - 滤镜->模糊->平均
    ![2.png](https://ooo.0o0.ooo/2016/11/12/582685e3ba65d.png)
- 设置背景图片为:

  ```
  .sample {
        /*略去其他设置*/
        background-image: url(https://ooo.0o0.ooo/2016/11/12/5826865399519.jpg),
                      linear-gradient(to bottom, #b9888c 34%, #bbcad5 77%, #b3a493 100%);
  }
  ```
  
  大功告成，此时网速慢的用户访问时，屏幕上会显示为:
  ![3.png](https://ooo.0o0.ooo/2016/11/12/5826886d4f333.png)
    
