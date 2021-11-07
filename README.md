# Girls-Frontline-emoji-for-waline [![](https://data.jsdelivr.com/v1/package/gh/Small-tailqwq/Girls-Frontline-emoji-for-waline/badge)](https://www.jsdelivr.com/package/gh/Small-tailqwq/Girls-Frontline-emoji-for-waline)
WaLine 的二次元表情包，取自 `B站` 
自己调了一些喜欢的自己用，注意！***无授权，非商用***

## 使用方法  

在客户端的 `WaLine` 配置下添加 `emoji` 的值为  
`https://cdn.jsdelivr.net/gh/Small-tailqwq/Girls-Frontline-emoji-for-waline@1.0/emoji/`  
即可  

具体参考 [WaLine官方文档](https://waline.js.org/guide/client/emoji.html#%E8%87%AA%E5%AE%9A%E4%B9%89%E8%A1%A8%E6%83%85)



> 问：emoji 图标很小啊，效果很差怎么办啊？  

答：建议在 html 代码处添加如下 css 代码，其中 `3.5em` 可以自行调整

```html
<style>
.v[data-class=v] .vcontent .vemoji {
    width: 3.5em !important;
}
</style>
```