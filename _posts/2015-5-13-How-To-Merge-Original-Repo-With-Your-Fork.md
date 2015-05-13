---
layout: post
permalink: /How-To-Merge-Original-Repo-With-Your-Fork
title: How to merge upstream/original repository with your forked repository
path: 2015-5-13-How-To-Merge-Original-Repo-With-Your-Fork.md
---

1. Add remote url as upstream

{% highlight bash %}
$ git remote add upstream https://github.com/barryclark/jekyll-now.git
{% endhighlight %}

- Then you can see the added url with:

{% highlight bash %}
$ git remote -v
{% endhighlight %}

2. Fetch upstream's changes

{% highlight bash %}
$ git fetch upstream
{% endhighlight %}


3. Merge upstream

 - If there's any change, merge it to your repository.

{% highlight bash %}
$ git merge upstream/master
{% endhighlight %}

 - When you encounter conflicts, edit those files personally and add/commit them.

4. Push to Github

{% highlight bash %}
$ git push origin master
{% endhighlight %}
