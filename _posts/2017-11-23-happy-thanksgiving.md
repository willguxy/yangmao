---
layout: post
title: Happy Thanksgiving
comments: true
post_id: 10001
categories: 
- Uncategorized
---

新博客的第一篇文章．大家感恩节快乐．感谢大家长久以来的关注

同时测试一下disqus评论系统



{% if page.comments %} 

<div id="disqus_thread"></div>
<script>

/**
*  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
*  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables*/

var disqus_config = function () {
this.page.url = 'http://yangmao.life/uncategorized/2017/11/23/happy-thanksgiving.html';  // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = 10001; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};

(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = 'https://yangmao.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>

{% endif %}

