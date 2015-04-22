---
layout: post
permalink: /tweet-sized-javascript-templating-engine
title: tweet-sized JavaScript templating engine
path: 2015-4-22-Tweet-Sized-Javascript-Templating-Engine.md
---

{% highlight javascript %}
// helper function
function t(s,d){
 for(var p in d)
   s=s.replace(new RegExp('{'+p+'}','g'), d[p]);
 return s;
}
{% endhighlight %}

* Calling it in code:

{% highlight javascript %}
t("Hello {who}! It's {time} ms since epoch.", { who: "JavaScript", time: Date.now });
// "Hello JavaScript! It's 1299680443046 ms since epoch."
{% endhighlight %}
