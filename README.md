# 2stabApe-emoji-for-waline [![](https://data.jsdelivr.com/v1/package/gh/Small-tailqwq/WaLine-emoji/badge)](https://www.jsdelivr.com/package/gh/Small-tailqwq/WaLine-emoji)
WaLine 的二次元表情包，取自 `B站` 
自己调了一些喜欢的自己用，注意！***无授权，非商用***

## 使用方法  

在客户端的 `WaLine` 配置下添加 `emoji` 的值为  

`https://cdn.jsdelivr.net/gh/Small-tailqwq/WaLine-emoji@1.1/%E5%B0%91%E5%89%8D%E5%B0%8F%E5%89%A7%E5%9C%BA/`  
`https://cdn.jsdelivr.net/gh/Small-tailqwq/WaLine-emoji@1.1/%E8%9B%86%E9%9F%B3%E5%A8%98/`

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
