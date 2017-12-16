---
layout: post
title: A much better way to automate tweeting Amex Offer
key: 20150801
tags:
- amex
- Amex
- amex offer
- twitter
---

之前bump into一些问题，导致所有的twitter账户被suspend，无奈一个个重新注册。每24小时内，每个ip可以注册一个twitter账户而不用手机号验证。所以可以用电脑连家里wifi注册一个，连手机热点注册一个，然后iphone设置里面注册一个。另外再多的话需要出门去星巴克之类的地方，或者找个VPN啥的。

之前的方法总结起来是这样的：

（1）利用IFTTT，将OffersBot的每条新推变成一篇新博客的标题

（2）利用twittersfeed把每篇新博客的标题变成一条tweet。

之前没有注意的是，每次新tweet都会把OffersBot的名字include进去。所以OffersBot一登陆……喝！这么多人at我。。。

最简单的方法就是把OffersBot的名字在IFTT里去掉，只保留tweet内容。但还是很奇怪，因为OffersBot毕竟是一个私人（死人）账户，他可能tweet任何东西，而我的账户每条都要跟他发一样的？！那就怪不得twitter关我账户了。

其实OffersBot也是从Amex官推上fetch data的，所以我们绕过他直接去fetch Amex的推特不就行了？等等。你去看Amex发的推特里并没有offer，反倒是一些宣传的东西，每天发无数条。。。你转这些有啥用？！Amex推的真正有用的东西在这里：

https://twitter.com/AmericanExpress/favorites

那怎么能fetch到favorites的东西呢？终于……我在这篇文章里找到了答案……

http://www.labnol.org/internet/twitter-rss-feed/28149/

上面这个东西你不需要看懂，因为我已经帮你看懂了，并且做好了准备工作。

如果你用我的方法，那么你要做的很简单。

（1）建立一个twitterfeed账户，然后创建一个feed机制。

（2）feed的来源
[在这里](https://script.google.com/macros/s/AKfycbxdQ2gI8-DFT3X9f7xs1S-YGjCPXrMpt0WF-eHfo-cL9nYpTh0/exec?627592612237737985)（你只需要copy url就行）（3）
**点击advance setting（非常重要！！！）你也不想被投诉然后被ban对吧？！然后选择include：description only。把post link的勾去掉。（看不清点大图）**

[![Screen Shot 2015-08-01 at 6.04.53 PM](https://willguxy.files.wordpress.com/2015/08/screen-shot-2015-08-01-at-6-04-53-pm.png?w=300)](https://willguxy.files.wordpress.com/2015/08/screen-shot-2015-08-01-at-6-04-53-pm.png)

（4）之后点下一步，把每个twitter账户加入列表（可以打开一个新的标签页，不停的登入登出，然后这边点authenticate twitter就行了。

（5）完成你的twitter feed。这样理论上来说，只要amex官推有新的favorite出来，你就可以自动推了，而且不会很奇怪的艾特amex的官推。

再次提醒，第三步注意设置，不然amex去twitter那边complain你，你的twitter账户可能被列为spam。