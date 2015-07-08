# SupportingMultipleScreens-Android

##屏幕适配新解Supporting Multiple Screens##
######以前是在屏幕密度后面指定具体的分辨率来区分，比如values-hdpi-800x480,layout-1280x720;>现在[官网](http://developer.android.com/guide/practices/screens_support.html)已经不建议这么去做,主要原因是目前android机器类型太多，显得不够灵活通用；现在建议方法是通过可用高度或者可用宽度来指定：


>######`values-h<sh>dp`
>######`values-w<sw>dp`

android在加载的时候会通过自身的dp=px/density(dp=800/1.5)或者相近的资源res去加载layout或values文件。
>例如：800x480px
>>values-h500dp 加载时设备会进入到此文件中去读取.
