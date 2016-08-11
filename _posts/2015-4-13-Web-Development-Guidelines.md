---
layout: post
title: Web Development Guidelines
---

## General guidelines and resources

* [Web Starter Kit](https://developers.google.com/web/starter-kit/) - by Google
* [Web Fundamentals](https://developers.google.com/web/fundamentals/) - by Google
* [Material design specification](http://www.google.com/design/spec/material-design/introduction.html) by Google  
* [Mozilla Developer Network](https://developer.mozilla.org/en-US/) - by Mozilla
* [Frontend Handbook](http://www.frontendhandbook.com/index.html) - by Cody Lindley
* [JavaScript Jargon](http://jargon.js.org/)
* [Free Programming Books](https://github.com/vhf/free-programming-books)

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
* [Essential JavaScript Links](https://github.com/ericelliott/essential-javascript-links) - by [ericelliott](https://github.com/ericelliott)
* [ES6 In Depth](https://hacks.mozilla.org/category/es6-in-depth/) - by Mozilla
* [ES6 Equivalents in ES5](https://github.com/addyosmani/es6-equivalents-in-es5) - by [@addyosmani](https://twitter.com/addyosmani)
* [ES6 Tools](https://github.com/addyosmani/es6-tools) - by [@addyosmani](https://twitter.com/addyosmani)
* [ES6 Tooling Tips](https://developers.google.com/web/shows/ttt/series-2/es2015?utm_source=feed&utm_medium=feed&utm_campaign=shows_ttt_feed) - by [@addyosmani](https://twitter.com/addyosmani)
* [ES6 Learning](https://github.com/ericdouglas/ES6-Learning) - by ericdouglas
* [JS Promises Playground](http://bevacqua.github.io/promisees) - by bevacqua
* [You Don't Need Jquery](https://github.com/oneuijs/You-Dont-Need-jQuery)

#### A Baseline for Front-End [JS] Developers: 2015
* [A Baseline for Front-End (JS) Developers: 2015](http://rmurphey.com/blog/2015/03/23/a-baseline-for-front-end-developers-2015/)

#### Chrome Dev Tools
* [Official documentation](https://developer.chrome.com/devtools) - by Google
* [Cheatsheet](http://anti-code.com/devtools-cheatsheet/) - by Jared Williams
* [Tips & Tricks](http://codepen.io/TheodoreVorillas/blog/chrome-devtools-tips-and-tricks) - by TheodoreVorillas
* [Demos & new features in Chrome Beta/Canary versions](https://speakerdeck.com/addyosmani/devtools-state-of-the-union-2015) - by [@addyosmani](https://twitter.com/addyosmani)
* [Blackboxing 3rd party libraries](https://developer.chrome.com/devtools/docs/blackboxing) - by Google
* [DevTools Tips](https://medium.com/google-developers/devtools-tips-for-sublime-text-users-cdd559ee80f8) - by Google

#### Front-end Tooling Workflow (Gulp.js, Bower, npm, linting etc..)

* [Introduction to modern JS Toolboox](http://www.infoq.com/articles/modern-javascript-toolbox?utm_source=telerik&utm_medium=email) - by David Haney
* [Package Managers: An Introductory Guide For The Uninitiated Front-End Developer](http://codylindley.com/techpro/2013_04_12__package-managers-an-introducto/) - by Cody Lindley
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
* [Visual Studio 2015 Shortcuts](http://visualstudioshortcuts.com/2015/)
* [Introduction to Visual Studio Debugging](http://blogs.msdn.com/b/visualstudio/archive/2015/08/11/introduction-to-debugging.aspx) - by Microsoft
* [Microsoft IE Developer Tools](http://dev.modern.ie/tools/) - by Microsoft
* [Browser Specific CSS and JavaScript Hacks](http://browserhacks.com/) - by Hugo Giraudel, Tim Pietrusky and Fabrice Weinberg
* [Must See JavaScript Dev Tools That Put Other Dev Tools to Shame](https://medium.com/javascript-scene/must-see-javascript-dev-tools-that-put-other-dev-tools-to-shame-aca6d3e3d925#.2dxeg7gyc)
* [Progressive Web Apps](https://developers.google.com/web/progressive-web-apps)
* [npm Resources And Tips](https://github.com/sindresorhus/awesome-npm?utm_source=javascriptweekly&utm_medium=email)

#### Cordova
* [Tools for Apache Cordova](http://blogs.msdn.com/b/visualstudio/archive/2015/06/01/tools-for-apache-cordova-samples-and-docs.aspx) - by Microsoft
* [Tools for Apache Cordova CLI Website](http://taco.tools/) - by Microsoft
* [Cordova CodePush plugin](http://microsoft.github.io/code-push/) - by Microsoft
* [Visual Studio Emulator for Android](https://www.visualstudio.com/en-us/features/msft-android-emulator-vs.aspx) - by Microsoft

#### AngularJS
* [Angular Styleguide](https://github.com/johnpapa/angular-styleguide) - by [@johnpapa](https://twitter.com/john_papa)
* [AngularJS Styleguide](https://github.com/toddmotto/angularjs-styleguide) - by [@toddmotto]( https://twitter.com/toddmotto )
* [Using AngularJS in Visual Studio 2013](http://blogs.msdn.com/b/visualstudio/archive/2015/02/05/using-angularjs-in-visual-studio-2013.aspx) - by [@JMatthiesen](https://twitter.com/JMatthiesen)
* [JavaScript IntelliSense for AngularJS in Visual Studio](https://github.com/jmbledsoe/angularjs-visualstudio-intellisense/) - by John Bledsoe
* [Angular 2 and TypeScript in Visual Studio](http://blogs.msdn.com/b/visualstudio/archive/2015/03/12/a-preview-of-angular-2-and-typescript-in-visual-studio.aspx) - by [@JMatthiesen](https://twitter.com/JMatthiesen)
* [Creating Line of Business applications using DNN and AngularJs](http://blog.webvoudig.nl/AppDevBlog/Post/753/Creating-Line-of-Business-applications-using-DNN-and-AngularJs)
* [Official Angular2 Style Guide](https://angular.io/styleguide?utm_source=javascriptweekly&utm_medium=email)

#### Kendo UI
* [Kendo UI Getting Started](http://codylindley.github.io/the-kendo-ui-book/) - by codylindley & Telerik
* [Kendo UI Mobile Guide](http://www.kendouimobileguide.com/) - by codylindley & Telerik

#### Ionic
* [Ionic + AngularJS Yeoman Generator](https://github.com/mwaylabs/generator-m-ionic) - by mwaylabs
* [Definitive 10,000 Word Guide to Ionic](http://tutorials.pluralsight.com/front-end-javascript/ionic-framework-a-definitive-10-000-word-guide?utm_source=javascriptweekly&utm_medium=email)

#### NodeJS
* [NodeJS in Visual Studio](http://blogs.msdn.com/b/visualstudio/archive/2015/04/24/node-js-tools-1-0-on-github-and-vms-available.aspx)
* [NodeJS Tools on GitHub](https://github.com/Microsoft/nodejstools)
* [Microsoft + Node.js Guidelines](https://github.com/MIcrosoft/nodejs-guidelines) - by Microsoft
* [Tutorial - Use latest NodeJS version in VS2015](http://ryanhayes.net/synchronize-node-js-install-version-with-visual-studio-2015/)

#### TypeScript
* [Getting Started with TypeScript](http://blog.teamtreehouse.com/getting-started-typescript?utm_source=telerik&utm_medium=email)
* [Using TypeScript in Visual Studio Code](http://blogs.msdn.com/b/typescript/archive/2015/04/30/using-typescript-in-visual-studio-code.aspx)
* [The repository for high quality TypeScript type definitions](http://definitelytyped.org/)

#### React
* [React Style Guide](https://github.com/Khan/style-guides/blob/master/style/react.md) - by Khan Academy
* [React Learning](http://www.reactjsprogram.com/)

#### Electron
* [Electron Quick Start](http://electron.atom.io/docs/tutorial/quick-start/)
* [Electron Tools & Resources](http://electron.atom.io/community/)

#### 2SexyContent
* [2sxc Snippets & Tricks](https://gist.github.com/jerkovicl/7bc090685103eab9e175)

## Git
* [Official GitHub Training](https://training.github.com/kit/) - by GitHub
* [Learn Git](http://schacon.github.io/gitbook/index.html)
* [Interactive Git Tutorial](http://gitimmersion.com/)
* [Video Tutorials](https://www.youtube.com/playlist?list=PL5-da3qGB5IBLMp7LtN8Nc3Efd4hJq0kD)
* [How to undo (almost) anything with Git](https://github.com/blog/2019-how-to-undo-almost-anything-with-git)
* [Coding in Windows - Setting Up Git & Cmder](http://www.awmoore.com/2015/01/14/coding-in-windows-part-1/)
* [Git Tips & Tricks](https://github.com/jbranchaud/til#git)


## Docker
* [Docker Tools for Visual Studio](https://github.com/Microsoft/DockerToolsDocs) - by Microsoft

## EntityFramework
* [Entity Framework Performance and What You Can Do About It](https://www.simple-talk.com/dotnet/.net-tools/entity-framework-performance-and-what-you-can-do-about-it/)

Compiled by ŠJ & LJ :fire:
