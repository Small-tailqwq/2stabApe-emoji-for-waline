# 2stabApe-emoji-for-waline ![logo](logo.png) [![](https://data.jsdelivr.com/v1/package/gh/Small-tailqwq/2stabApe-emoji-for-waline/badge)](https://www.jsdelivr.com/package/gh/Small-tailqwq/2stabApe-emoji-for-waline)
适配 WaLine 的 *第三方* 二次元表情包，来源为 [Bilibili](https://www.bilibili.com) 或者 [AcFun](https://acfun.cn) 


  
***注意！注意！注意！注意！注意！注意！注意！注意！注意！注意！***  
***本库表情包未获得任何授权，禁止任何组织或个人以任何形式的商用***

## 使用方法  

> 可参考[官方文档](https://waline.js.org/reference/component.html#emoji)  

进入这个链接，选择自己想要的表情包点进去，复制 url 栏的链接填入 Waline 即可  
```
https://cdn.jsdelivr.net/gh/Small-tailqwq/2stabApe-emoji-for-waline@1.1.1/
```

### 关于 jsdelivr 爆炸

之前 jsd 的 cdn 全面爆炸了，如果有需要可以使用我自己提供的国内 CDN  
把 `cdn.jsdelivr.net` 替换为 `hayasa.skadi.top` 即可
> 当然，能 cdn 的仅限我这个表情包库（不然呢？）
且最新的表情可能得等我手动同步


*顺带一提之前好像有哪个表情包有问题来着，不过现在也已经忘了，如果在使用时发现了记得开个 issues 提醒我一下*


## 你问我答

> emoji 图标很小啊，效果很差怎么办啊？  

我的建议是，在 html 代码处添加如下 css 代码，其中 `3.5em` 可以自行调整  
另外 waline2 之后对样式名称有些许改变，改一改继续用~

```html
// waline2 之前的版本
<style>
    .v[data-class=v] .vcontent .vemoji {
        width: 3.5em !important;
    }
</style>
// waline2 之后的版本
<style>
    .wl-content .vemoji, .wl-content .wl-emoji {
        height: 3.5em !important;
    }
</style>
```
> 表情候选框里的表情也好小啊，都看不清

我的建议是，同样更改 css 样式。其中参数可以自行在F12内调整尝试再进行修改，最好确保移动端不会太大，PC端不会太小。
```html
// waline2 之前的版本
<style>
    .v[data-class=v] .vemoji-popup .vemoji {
    max-width: 2em !important;
    max-height: 3.5em !important;
}
</style>
// waline2 之后的版本
<style>
    .wl-emoji-popup .wl-emoji {
        max-width: 2em !important;
        max-height: 3.5em !important;
    }
</style>
```

> 为什么表情包基本全是中文，url 都不好分辨

不会英文，懒得翻译，再说老外应该也没有这方面的需求。url 方面直接用中文就完事了呗，`又不是不能用.jpg`  

> 不懂啊，那你能帮帮我吗

看图 
~~哦，这当然是一张老图，但是不影响理解就是了~~ 
![截图001](/%E6%88%AA%E5%9B%BE001.png)

## 更新日志

*2022-08-10*  
`[+]` 更新了塔菲表情包喵，包括粉丝装扮以及直播间表情，未来可能还会更新其他管人的表情，不过得找有粉丝装扮的猴米毛才行（自己没买）

*2022-05-19*  
`[~]` 连夜把表情包丢 oss 上了，不知道阿里那玩意一年得花多少钱，合适就继续搞，当然你也可以直接下载下来自己丢服务器上。  



*2021-11-08*  
`[+]` 添加了 A站 目前 *网页版所有的* 表情包，由于数量过于庞大可能存在 bug。如果遇到了欢迎反馈    
* 新建文本文档是A站给的表情包，有时间按类型去重再整合一下，嫌我慢也可以自己下下来整
