# Bitmap 详解

## 压缩质量参数

这都是色彩的存储方法：我们知道ARGB指的是一种色彩模式，里面A代表Alpha，R表示red，G表示green，B表示blue，其实所有的可见色都是右红绿蓝组成的，所以红绿蓝又称为三原色，每个原色都存储着所表示颜色的信息值

说白了其实就是：

- ALPHA_8就是Alpha由8位组成
- ARGB_4444就是由4个4位组成即16位，
- ARGB_8888就是由4个8位组成即32位，
- RGB_565就是R为5位，G为6位，B为5位共16位

由此可见：

- ALPHA_8 代表8位Alpha位图
- ARGB_4444 代表16位ARGB位图
- ARGB_8888 代表32位ARGB位图
- RGB_565 代表16位RGB位图

位图位数越高代表其可以存储的颜色信息越多，当然图像也就越逼真。