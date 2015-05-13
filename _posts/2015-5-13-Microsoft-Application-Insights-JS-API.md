---
layout: post
permalink: /microsoft-application-insights-js-api.md
title: Microsoft Application Insights JS API
path: 2015-5-13-Microsoft-Application-Insights-JS-API.md
tags:
- insights
- javascript
published: true
---

**Since there is no official documentation, here is the proper setup to enable Microsoft Application Insights for Javascript/Cordova apps and websites:**

#### 1. In the Azure portal, create a new Application Insights resource:

![Azure](https://acomdpsstorage.blob.core.windows.net/dpsmedia-prod/azure.microsoft.com/en-us/documentation/articles/app-insights-javascript/20150508050839/01-create.png)

#### 2. Get the snippet from Quick Start section:

![Quick Start](https://acomdpsstorage.blob.core.windows.net/dpsmedia-prod/azure.microsoft.com/en-us/documentation/articles/app-insights-javascript/20150508050839/02-monitor-web-page.png)

#### 3. Insert the script snippet just before the <code></head></code> tag of every page you want to track:

- In an ASP.NET MVC project, you'd put it in View\Shared_Layout.cshtml

- If your JavaScript app isn't a web page - for example, if it's a Cordova app or a Windows Runtime app using JavaScript - insert an extra line after the instrumentation key:

{% highlight javascript %}
...{
    instrumentationKey:"00000000-662d-4479-0000-40c89770e67c",
    endpointUrl:"https://dc.services.visualstudio.com/v2/track"
} ...
{% endhighlight %}

- For AngularJS there's an [AngularJS module](http://ngmodules.org/modules/angular-appinsights).

- If you want to check the telemetry that a web app/site is sending to Application Insights, check with debugging tools for requests sent to **dc.services.visualstudio.com**.

#### 4. API Methods

- Send page views:

{% highlight javascript %}
appInsights.trackPageView("name");
appInsights.trackPageView("name", "url");
appInsights.trackPageView("name", "url", { prop: "p1" }); 
{% endhighlight %}

- Send events:

{% highlight javascript %}
appInsights.trackEvent("exampleEvent1");
appInsights.trackEvent("exampleEvent2", { exampleEventProperty1: "test", another: "test2" });
appInsights.startTrackEvent("exampleTimedEvent");
setTimeout(function() { 
  appInsights.stopTrackEvent("exampleTimedEvent"); 
}, 1000);
{% endhighlight %}

- Send metrics:

{% highlight javascript %}
appInsights.trackMetric("metricName", 42);
appInsights.trackMetric("metricName", 42, { prop: "test" });
{% endhighlight %}

- Send traces:

{% highlight javascript %}
appInsights.trackTrace("trace message 1");
appInsights.trackTrace("trace message 2", { prop: "test" });
{% endhighlight %}

- Send exceptions:

{% highlight javascript %}
appInsights.trackException("error message1");
appInsights.trackException(new Error("error message2"));
appInsights.trackException(new Error("error message2"), "locationWhereThisWasHandled?");
appInsights.trackException(new Error("error message3"), null, { prop: "test" });
{% endhighlight %}
