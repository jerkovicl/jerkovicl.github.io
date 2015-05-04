---
layout: post
permalink: /adding-javascript-intellisense-to-vs-code
title: Adding Javascript Intellisense for projects in Visual Studio Code
path: 2015-5-4-Adding-Javascript-Intellisense-To-VS-Code.md
---

- Consolidating all typings definition for JS libs into one file:

{% highlight javascript %}
npm install tsd -g
# cd to your project folder
tsd query -r -o -a install angular jquery node --save
{% endhighlight %}

- This produces a tsd.d.ts file which you can reference in your JavaScript files to get intellisense like this:

{% highlight javascript %}
/// <reference path="/typings/tsd.d.ts" />
{% endhighlight %}
