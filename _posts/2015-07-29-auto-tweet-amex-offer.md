---
layout: article
title: 【秘籍】自动推Amex offer
comment: true
key: 20150729
tags: AMEX AmexOffer twitter
---

**福利来了，这次是独家的，微博我都不发这篇了。**

最近几个可推的Amex offer搞的大家很蛋疼吧。早上醒来一看论坛，喝！早就推满了！不知道是僧多粥少还是太多人设置了自动发推。最早之前大家都知道可以用offersbot，不过在被推特ban了以后，这个app也无限期停摆了。

其实稍微懂点tech的人都知道怎么work的，无非就是fetch Amex的官方推特，然后自己也发同样的内容。最理想的状态是以高的刷新频率来fetch，然后可以第一时间sign up。既然原理大家都懂了，高手可以自己做一些脚本来搞。

这里我用的方法比较小白。


首先我尝试了IFTTT。但有一个问题是IFTTT只支持一个推特账户，也就是说如果你有几十个的话，要新建几十个IFTTT账户。慢慢建倒也不着急，反正recipe加上去就不用动了。


第二种方法（稍微）省去了set-up的时间。这里我只用一个IFTTT账户，IF（offersbot发一条推特）THEN（我在blogspot上建立一篇博客）。博客的标题就是offersbot发的推特内容。这里不知道IFTTT fetch的时间间隔是多久。


然后你需要一个免费的东东叫twitterfeed（http://twitterfeed.com/），注册一个账户，然后建立一条new feed。这里feed来源就是你的blogspot rss。输出就是twitter账户。有意思的是twitterfeed允许你在一条feed里加入多个twitter账户。比如我现在有14个，做法是：连接一个推特账户，登出现有twitter，再登入下一个twitter账户，然后回到twitterfeed再次添加，如此反复，知道把所有账户都加到这条feed里。

然后你可以测试一下。比如我新建一篇博客，标题是#AmexHP。回到twitterfeed里点check now，不一会儿就可以看到自己推特上发了一条新推，#AmexHP以及后面一些没用的blablabla。


**注意：这个方法速度并不快，因为twitterfeed最快的fetch速度是每30分钟，算上IFTTT的延迟，预计一小时内可以完成，可以适应大部分Amex offer。如果你嫌慢，那就一个一个set-up你的IFTTT吧。**
