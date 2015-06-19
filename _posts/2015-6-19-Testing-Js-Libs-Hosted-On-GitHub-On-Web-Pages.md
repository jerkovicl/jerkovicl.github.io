---
layout: post
permalink: /testing-js-libs-hosted-on-github-on-web-pages
title: Testing JS libraries hosted on GitHub on web pages
path: 2015-6-19-Testing-Js-Libs-Hosted-On-GitHub-On-Web-Pages.md
tags:
- github
- testing
- javascript
- rawgit
published: true
---

Sometimes you just need to use some scripts for testing or making some demos.  
For that purposes you can inject scripts using this approach:

- Find the wanted script on GitHub and copy its url
- Go to website [RawGit](https://rawgit.com/) and paste url there
- For dev/testing structure url like this __https://rawgit.com/user/repo/branch/file__ and for production like this __https://cdn.rawgit.com/user/repo/tag/file__
- Open Firefox and bring the Developer Toolbar with __Shift+F2__ keyboard shortcut
- Type {% highlight javascript %}inject https://rawgit.com/username/repo/branch/folder/file.min.js{% endhighlight %}
