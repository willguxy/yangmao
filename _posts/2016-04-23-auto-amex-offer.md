---
layout: article
title: 【geek向】自动添加Amex Offer
comment: true
key: 20160423
tags: AMEX AmexOffer tip
---

首先，我曾经发过数篇文章来介绍和解释一个自动推amex offer的工具，基本原理就是通过twitterfeed来自动发出跟offersbot一样的内容，来为你的卡加上amex offer。目前这个工具我还在使用，而且完全hassle-free，不需要我来管理任何东西。

今天想给大家介绍自动添加amex offer的另一个层面：把进入你的amex账户点击『add to card』这个操作变成完全自动化。

如果你觉得我之前说的东西有点极客，理解不了，那么可能下面我要介绍的全新工具已经不适合你了，毕竟技术门槛又提高了一个层面。硬币的另一面是，真的set up好之后，你可以省下不少的管理成本。

做这样一个工具的初衷是因为手里的Amex卡已经很多了。我在微博上做了粗略的估计：一般情况是，每个非单身狗跟自己的另一半，各有4+张Amex卡——credit卡和charge卡加起来6~8张也很正常。按每人6张主卡算吧，你跟另一半再把对方加为副卡，一共24+张Amex卡。至于撸的狠的，再加几个亲戚朋友为副卡，三四十张也不足挂齿吧。

这么多卡，管理起来非常的不便，倒不是说用起来麻烦——刷卡是无所谓了，还款的时候盯着主卡还就行了。主要问题是加offer和记录情况哪张卡有哪个offer。现在不少offer都是targeted，一张一张登陆去查看，非常费时费力。

因为我写了一个python的小程序，结合selenium网页测试工具，可以在后台自动运行，把账户的offer自动加好，并且生成log文件记录。GitHub地址如下：

https://github.com/willguxy/AutoAmex

有一个问题不得不面对的就是，如果你完全看不懂这个简单的程序，出了问题你就完全没法debug。所以只建议有一些基础能figure out的童鞋使用。另外把账户登录信息存在csv文件里是一件非常危险的事情，这里面涉及的风险我是完全不会负责任的。如果你水平够高，自己加一个加密算法也是可以的。

目前貌似还有点小问题，偶尔会miss几个offer，但运行第二次的时候就会把miss的都加上了。哪位读者能够优化一下程序的话，我也会很感激。

Enjoy。
