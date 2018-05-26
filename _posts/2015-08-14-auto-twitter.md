---
layout: article
title: AutoTweet最终形态
comment: true
key: 20150814
tags: AMEX AmexOffer twitter
---

之前写了twitter自动推Amex Offer的系列文章，
**[最终成品在此](https://willguxy.wordpress.com/2015/08/01/a-much-better-way-to-automate-tweeting-amex-offer/)**。


**大致意思是：等待Amex/favorites的列表更新，一旦更新便会产生一条feed。这条feed被twitterfeed.com识别，并在你的所有twitter账户上发出相同的内容。**

后来发现一些小问题，主要是Amex/favorites更新并不及时。一条hashtag生效后几个小时才会更新。这样的话如果是非常popular的offer，在加到自己卡上就已经被推满了。

所以最理想的方法是这样的：
**建立一个list，收集所有AmexOffers账号回复的推特中提到的Hashtag。大家可以看到，这个账号的回复非常频繁，基本每1-2秒一条。你不能全部都转发，这样twitter瞬间就把你账号封掉了。所以你的list用来储存这些hashtag，只有当一条新回复中包含了这个list中没有的hashtag，你再发这条tweet。**
也就是说一旦有人成功推了一个offer，你的list就会更新，并且你会推那个offer。

可惜我JavaScript能力有限，还没太看懂原帖里的那个脚本，所以也无从修改。

不过好在我跟OffersBot的制作人简单聊了一下，发现OffersBot也用了类似的机理。所以最终版本的自动tweet，还是需要和OB发一样的东西。好在OB并不常发些没用的，所以你就尽管推吧。


**[feed的url链接在此](https://script.google.com/macros/s/AKfycbyMQg7m5eAwBgjh31GpxmCTTNmF1wkRTlDQn7WW-l9i4vFX5fwd/exec?631004517006471168)**


**最后记得在设置里选“Description Only”。真的真的要记得。**
