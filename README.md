# 2stabApe-emoji-for-waline ![logo](logo.png) [![](https://data.jsdelivr.com/v1/package/gh/Small-tailqwq/WaLine-emoji/badge)](https://www.jsdelivr.com/package/gh/Small-tailqwq/WaLine-emoji)
适配 WaLine 的 *第三方* 二次元表情包，来源为 [Bilibili](https://www.bilibili.com) 或者 [AcFun](https://acfun.cn) 


  
***注意！注意！注意！注意！注意！注意！注意！注意！注意！注意！***  
***本库表情包未获得任何授权，禁止任何组织或个人以任何形式的商用***

## 使用方法  

进入这个链接，选择自己想要的表情包点进去，复制 url 填入即可  
```
https://cdn.jsdelivr.net/gh/Small-tailqwq/WaLine-emoji@1.1.1/
```

### 关于 jsdelivr 爆炸

最近大伙也基本都发现了 `cdn.jsdelivr.net` 被 dns 污染一事吧，我也换掉了自己网站上的 js 啥的就是了
顺带给这表情包丢阿里云的 OSS 里了，大陆访问速度很不错，原来有用这表情包的把 `cdn.jsdelivr.net` 换成 `hayasa.oss-cn-hangzhou.aliyuncs.com` 即可

*顺带一提之前好像有哪个表情包有问题来着，不过现在也已经忘了，有记得的提醒我一下*

具体配置可以参考 [WaLine官方文档](https://waline.js.org/guide/client/emoji.html#%E8%87%AA%E5%AE%9A%E4%B9%89%E8%A1%A8%E6%83%85)


## 你问我答

> emoji 图标很小啊，效果很差怎么办啊？  

我的建议是，在 html 代码处添加如下 css 代码，其中 `3.5em` 可以自行调整

```html
<style>
.v[data-class=v] .vcontent .vemoji {
    width: 3.5em !important;
}
</style>
```
> 表情候选框里的表情也好小啊，都看不清

我的建议是，同样更改 css 样式。其中参数可以自行在F12内调整尝试再进行修改，最好确保移动端不会太大，PC端不会太小。
```html
<style>
    .v[data-class=v] .vemoji-popup .vemoji {
    max-width: 2em !important;
    max-height: 3.5em !important;
}
</style>
```

> 为什么表情包基本全是中文，url 都不好分辨

我不会英文，懒得翻译，再说老外应该也没有这方面的需求。url 方面先忍忍，`又不是不能用.jpg`  


## 更新日志

*2021-11-08*  
`[+]` 添加了 A站 目前 *网页版所有的* 表情包，由于数量过于庞大可能存在 bug。如果遇到了欢迎反馈    
* 新建文本文档是A站给的表情包，有时间按类型去重再整合一下，嫌我慢也可以自己下下来整
