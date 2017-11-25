---
layout: post
title: 如何建立mitbbs的RSS feed
#permalink: https://willguxy.wordpress.com/2016/01/10/如何建立mitbbs的rss-feed/index.html
post_id: 792
categories: 
- miscellaneous
- Uncategorized
---

大家在买买提二手版经常买卖东西的话，可能会想第一时间知道市场上某个产品在待售或者求购，以及价格是多少。所以在这里我给大家提供一个小trick，可以收到新帖（其实是顶帖）的通知，并且可以过滤关键词。

举例来说，二手版的RSS feed是下面这个网址：

http://www.mitbbs.com/board_rss/fleamarket.xml

任何一个RSS阅读器都可以添加这个源，有些好用一点的自带过滤功能，这个我先不提。如果您工具已经ready，可以直接上。

我的办法是这样的：先利用IFTTT，将任何新的帖子自动转发到我的邮箱里。这里可以设置一个过滤关键词，比如『求购』。然后在我的Gmail里继续设置过滤词。注意这里Gmail收到邮件的发件人是你自己，所以只需要过滤所有来自你自己的邮件。比如你想继续过滤，并且只关注求购GC的帖子，那么设置包含『求购』，且不包含『GC』，action选择直接删除即可。这样的话不符合条件的邮件自动被删除（或者归档），保留下来的邮件就是『求购GC』的邮件啦。

当然如果你是GC买家，也可以把『求购』替换成出售。或者你是医护人员，可以加入关键词『label』，甚至你感兴趣的产品型号等等。

总结起来就是在已经有RSS源的情况下，先IFTTT，再在Gmail里设置过滤。这样收到的邮件带一个地址，可以点开。

注意：前面的RSS源，可以替换成任意版面。暂时没找到Re帖列表的RSS。有任何问题欢迎留言。

以上。