---
layout: post
title: Web Development Guidelines
---

## General guidelines and resources

* [Web Starter Kit](https://developers.google.com/web/starter-kit/) - by Google
* [Web Fundamentals](https://developers.google.com/web/fundamentals/) - by Google
* [Material design specification](http://www.google.com/design/spec/material-design/introduction.html) by Google  
* [Mozilla Developer Network](https://developer.mozilla.org/en-US/) - by Mozilla

## HTML / CSS guidelines

* [CSS Guidelines](http://cssguidelin.es/) - by [@csswizardry](https://twitter.com/csswizardry)
* [Code Guide](http://codeguide.co/) - by [@mdo](https://twitter.com/mdo)
* [WTF HTML CSS](http://wtfhtmlcss.com/) - by [@mdo](https://twitter.com/mdo)
* [CSS References](http://tympanus.net/codrops/css_reference/) - Codrops

#### ARIA roles
[WAI-finding with ARIA Landmark Roles](http://alistapart.com/column/wai-finding-with-aria-landmark-roles)

#### Preprocessors
* [LESS.js documentation](http://lesscss.org/)
* [LESSHat mixins documentation](https://github.com/madebysource/lesshat/blob/master/README.md) 
* [Sass / SCSS documentaion](http://sass-lang.com/documentation/file.SASS_REFERENCE.html)

#### Moj stil pisanja HTML-a / CSS-a -- BEM metodologija

{% highlight css %}
// block-name
// block-name--modifier-name
// block-name__element-name
// block-name__element-name--modifier-name
{% endhighlight %}

##### Primjer u praksi


{% highlight html %}
<nav class="main-nav" role="navigation">
    <ul class="main-nav__list">
         <li class="main-nav__item main-nav__item--has-child">
              <a href="/Home" class="main-nav__link main-nav__link--parent" title="Home">
                   Home
             </a>
         </li>
    </ul>
</nav>
{% endhighlight %}

## JavaScript guidelines

#### ES5 i ES6
* [Learning JavaScript Design Patterns](http://addyosmani.com/resources/essentialjsdesignpatterns/book/) - by [@addyosmani](https://twitter.com/addyosmani)
* [ES6 (latest) guidelines](https://github.com/airbnb/javascript/tree/es6) - by Airbnb
* [ES5 guidelines](https://github.com/airbnb/javascript/tree/es6/es5) - by Airbnb
* [Native JS Functions, Helpers & Plugins](http://plainjs.com/javascript/?utm_source=javascriptweekly&utm_medium=email) - by plainJS

#### A Baseline for Front-End [JS] Developers: 2015
* [A Baseline for Front-End (JS) Developers: 2015](http://rmurphey.com/blog/2015/03/23/a-baseline-for-front-end-developers-2015/)

#### Chrome Dev Tools
* [Official documentation](https://developer.chrome.com/devtools) - by Google
* [Cheatsheet](http://anti-code.com/devtools-cheatsheet/) - by Jared Williams
* [Tips & Tricks](http://codepen.io/TheodoreVorillas/blog/chrome-devtools-tips-and-tricks) - by TheodoreVorillas
* [Demos & new features in Chrome Beta/Canary versions](https://speakerdeck.com/addyosmani/devtools-state-of-the-union-2015) - by [@addyosmani](https://twitter.com/addyosmani)
* [Blackboxing 3rd party libraries](https://developer.chrome.com/devtools/docs/blackboxing) - by Google

#### Front-end Tooling Workflow (Gulp.js, Bower, npm, linting etc..)

* [Introduction to modern JS Toolboox](http://www.infoq.com/articles/modern-javascript-toolbox?utm_source=telerik&utm_medium=email) - by David Haney
* [Build Automation](https://speakerdeck.com/addyosmani/front-end-tooling-workflows) - by [@addyosmani](https://twitter.com/addyosmani)
* [Bower](http://blog.teamtreehouse.com/getting-started-bower) - by [Treehouse](https://teamtreehouse.com/)
* [Gulp](http://andy-carter.com/blog/a-beginners-guide-to-package-manager-bower-and-using-gulp-to-manage-components) - by Andy Carter
* [Project scaffolding with Yeoman](http://yeoman.io/blog/state-of-the-moustache-2015.html) - by [@addyosmani](https://twitter.com/addyosmani)
* [Brackets Extensions](http://www.johnpapa.net/my-recommended-brackets-extensions/) - by [@johnpapa](https://twitter.com/John_Papa)
* [Gulp Starter kit](https://github.com/jerkovicl/gulp-starter-kit) - WIP
* [Using WebPack as Module Loader](http://developer.telerik.com/featured/webpack-for-visual-studio-developers/) - by [Burke Holland](http://twitter.com/burkeholland)
* [Using RequireJS with Visual Studio](http://blogs.msdn.com/b/visualstudio/archive/2015/04/20/using-requirejs-with-visual-studio.aspx) - by [@JMatthiesen](https://twitter.com/JMatthiesen)
* [Customizing IntelliSense for RequireJS](https://msdn.microsoft.com/en-us/library/dn904583.aspx) - by [@JMatthiesen](https://twitter.com/JMatthiesen)
* [Using Grunt and Bower in Visual Studio 2015](http://www.asp.net/vnext/overview/aspnet-vnext/grunt-and-bower-in-visual-studio-2015) - by Mike Wasson
* [JavaScript Web Tools with Visual Studio 2015 and ASP.NET 5](http://www.microsoft.com/en-us/download/details.aspx?id=46417&CR_CC=200619609) - by Microsoft
* [Understanding the Manifest for Web App](http://www.thishereweb.com/understanding-the-manifest-for-web-app/) - by Microsoft
* [Building Hosted Web Apps with ManifoldJS](http://www.thishereweb.com/manifoldjs-building-simple-hosted-web-apps/) - by Microsoft
* [Visual Studio Tips & Tricks](http://blogs.msdn.com/b/benwilli/archive/2015/04/07/back-to-basics-visual-studio-tips.aspx) - by BenWilli
* [Microsoft IE Developer Tools](http://dev.modern.ie/tools/) - by Microsoft
* [Browser Specific CSS and JavaScript Hacks](http://browserhacks.com/) - by Hugo Giraudel, Tim Pietrusky and Fabrice Weinberg
* [Tools for Apache Cordova](http://blogs.msdn.com/b/visualstudio/archive/2015/06/01/tools-for-apache-cordova-samples-and-docs.aspx) - by Microsoft

#### AngularJS
* [Angular Styleguide](https://github.com/johnpapa/angular-styleguide) - by [@johnpapa](https://twitter.com/john_papa)
* [AngularJS Styleguide](https://github.com/toddmotto/angularjs-styleguide) - by [@toddmotto]( https://twitter.com/toddmotto )
* [Using AngularJS in Visual Studio 2013](http://blogs.msdn.com/b/visualstudio/archive/2015/02/05/using-angularjs-in-visual-studio-2013.aspx) - by [@JMatthiesen](https://twitter.com/JMatthiesen)
* [JavaScript IntelliSense for AngularJS in Visual Studio](https://github.com/jmbledsoe/angularjs-visualstudio-intellisense/) - by John Bledsoe
* [Angular 2 and TypeScript in Visual Studio](http://blogs.msdn.com/b/visualstudio/archive/2015/03/12/a-preview-of-angular-2-and-typescript-in-visual-studio.aspx) - by [@JMatthiesen](https://twitter.com/JMatthiesen)

#### Kendo UI
* [Kendo UI Getting Started](http://codylindley.github.io/the-kendo-ui-book/) - by codylindley & Telerik
* [Kendo UI Mobile Guide](http://www.kendouimobileguide.com/) - by codylindley & Telerik

#### NodeJS
* [NodeJS in Visual Studio](http://blogs.msdn.com/b/visualstudio/archive/2015/04/24/node-js-tools-1-0-on-github-and-vms-available.aspx)
* [NodeJS Tools on GitHub](https://github.com/Microsoft/nodejstools)

#### TypeScript
* [Getting Started with TypeScript](http://blog.teamtreehouse.com/getting-started-typescript?utm_source=telerik&utm_medium=email)
* [Using TypeScript in Visual Studio Code](http://blogs.msdn.com/b/typescript/archive/2015/04/30/using-typescript-in-visual-studio-code.aspx)
* [The repository for high quality TypeScript type definitions](http://definitelytyped.org/)

Compiled by ŠJ & LJ :fire:
