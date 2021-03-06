星际移民时间线
===============

星际移民时间线，[在线浏览地址在此](http://interimm.github.io/timeline/)。



如何录入和修改数据内容
------------------------

数据文件是 JSONP 文件，用 JSONP 是为了方便别人跨域使用。


这里是一个数据文件的示例：


```
storyjs_jsonp_data = {
    "timeline":
    {
        "headline":"星际移民时间线",
        "type":"default",
		    "text":"星际移民时间线列举了星际移民历史上的诸多重大事件。",
		    "startDate":"1900",
        "date": [
            {
                "startDate":"2027",
                "headline":"人类首次登陆火星",
                "text":"<p>人类的脚印首次镌刻在了这颗红色星球上，3名宇航员在<a href='https://github.com/InterImm/InterImmBook/blob/master/book/resources/landing_spot.png' target='_blank'>着陆点</a>附近（23.27°N 109.08°E，位于火星第九区、即阿蒙蒂斯区，地处乌托邦平原边缘）开展了为期300天的科学探测活动，采集了大量火星土壤、岩石样品，最终于2029年返回地球。人类登上火星的那一天（地球纪元2027年7月23日）被定为火星纪元元年1月1日</p>",
                "asset":
                {
                    "media":"https://raw.githubusercontent.com/InterImm/InterImmBook/master/book/resources/landing_spot.png",
                    "credit":"",
                    "caption":""
                }
            },
            {
                "startDate":"",
                "headline":"",
                "text":"<p></p>",
                "asset":
                {
                    "media":"",
                    "credit":"",
                    "caption":""
                }
            }
        ]
    }
}
```


语言的设置，常用的是：


`lang`
Localization
*default is `en` English*

* `en` *English*
* `zh-ch` *Chinese*
* `zh-tw` *Taiwanese*


`"startDate":"1900"` 用来设置开始的时间。


`"media":""` 里面可以直接使用 Twitter, YouTube, Flickr, Instagram, TwitPic, Wikipedia, Dailymotion, SoundCloud and Vimeo，当然也可以直接使用图片链接。


这里面可以使用 HTML 代码，但是注意 `"` 的使用，应该使用 `'` 或者 `'''` 来避免跟 JSON 格式冲突。

更多的设置可以参考 [TimelineJS](https://github.com/NUKnightLab/TimelineJS) 在移交给 KnightLab 之前的说明文件，虽然现在那个 repo 已经被删除了，但是我之前 fork 的时候留了[一份](MANUAL.md)。


建议
-------------

为避免 gh-pages 页面出现问题，导致别人无法浏览，添加或者修改的时候应该建立新的分支，在本地测试无误之后再合并到 gh-pages 分支中来。

如果对于这个有疑问，可以在 Issues 中提问，然后大家来讨论具体的操作。

-------------
詢問 是否坐在游戲内又如何？
-------------
