# 记录一些获取ipa的一些方式

## 一、使用浏览器

获取安装地址，使用`Chrome`打开，如下图

![](https://user-images.githubusercontent.com/16829768/58883998-1a2f9d80-8712-11e9-988a-616c0a1fb471.jpg)


如果你看到类似`itms-services://?action=download-manifest&url=https://xxx.plist`，那么直接复制url后面的地址`https://xxx.plist`，再次使用`Chrome`打开，会发现会下载一个同名的`xxx.plist`

![](https://user-images.githubusercontent.com/16829768/58883999-1a2f9d80-8712-11e9-8bfc-92d6567f30f0.jpg)


下面这个就是`ipa`的地址了.

这种方式基本上可以解决大部分的情况了,比如通过`fir`下载的都可以通过这种方式。

## 二、通过TestFlight安装的

如果你是通过抓包的方式的话，会找到一个类似这样的地址


```
http://iosapps.itunes.apple.com/apple-assets-us-std-000001/Purple113/v4/4d/df/ed/4ddfed8e-a045-950a-7777-90f091a1015f/pre-thinned8061960359639124299.thinned.signed.beta.ipa?accessKey=1557998079_6365517050277735400_kN8Vf4%2FnJKHeuCosh1rx7X%2FgXVm%2FOdjZn5aa2jtHnWaNZUO%2FrpxheJSJMNPZMLfBZIrsWPpX%2BS%2BTXMW%2Bpzku4Ga%2BdDnYBSJ3oj3%2B6WZkJk4rTYNCganhUUM06DYVsp4QiZc2O2O4KqUScCay%2FnKaT8HsyGPitgKLId9TqzQEvW5YEEvWTqmm4jkVDXOPZZeeb8QXX%2Fzv6DXZ1Fu3PHWk%2Bpct8kAPQ431N9Z%2Bj1VG%2BQ4%3D

```

遗憾的是这个包无法解析，我猜测这是个壳程序。

这种方式安装的app想要抓取ipa，我目前没有找到很好的方式，一般都是通过在越狱手机上安装的，然后倒入ipa。




