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

#### A Baseline for Front-End [JS] Developers: 2015
* [A Baseline for Front-End (JS) Developers: 2015](http://rmurphey.com/blog/2015/03/23/a-baseline-for-front-end-developers-2015/)

#### Chrome Dev Tools
* [Official documentation](https://developer.chrome.com/devtools) - by Google
* [Cheatsheet](http://anti-code.com/devtools-cheatsheet/) - by Jared Williams
* [Tips & Tricks](http://codepen.io/TheodoreVorillas/blog/chrome-devtools-tips-and-tricks) - by TheodoreVorillas
* [Demos & new features in Chrome Beta/Canary versions](https://speakerdeck.com/addyosmani/devtools-state-of-the-union-2015) - by [@addyosmani](https://twitter.com/addyosmani)
* [Blackboxing 3rd party libraries](https://developer.chrome.com/devtools/docs/blackboxing) - by Google

#### Front-end Tooling Workflow (Gulp.js, linting etc..)

* [Introduction to modern JS Toolboox](http://www.infoq.com/articles/modern-javascript-toolbox?utm_source=telerik&utm_medium=email) - by David Haney
* [Build Automation](https://speakerdeck.com/addyosmani/front-end-tooling-workflows) - by [@addyosmani](https://twitter.com/addyosmani)
* [Bower](http://blog.teamtreehouse.com/getting-started-bower) - by [Treehouse](https://teamtreehouse.com/)
* [Gulp](http://andy-carter.com/blog/a-beginners-guide-to-package-manager-bower-and-using-gulp-to-manage-components) - by Andy Carter
* [Brackets Extensions](http://www.johnpapa.net/my-recommended-brackets-extensions/) - by [@johnpapa](https://twitter.com/John_Papa)
* [Gulp Starter kit](https://github.com/jerkovicl/gulp-starter-kit) - WIP

#### AngularJS
* [Angular Styleguide](https://github.com/johnpapa/angular-styleguide) - by [@johnpapa](https://twitter.com/john_papa)
* [AngularJS Styleguide](https://github.com/toddmotto/angularjs-styleguide) - by [@toddmotto]( https://twitter.com/toddmotto ) 

#### Kendo UI
* [Kendo UI Getting Started](http://codylindley.github.io/the-kendo-ui-book/) - by codylindley & Telerik
* [Kendo UI Mobile Guide](http://www.kendouimobileguide.com/) - by codylindley & Telerik

Compiled by ŠJ & LJ :fire:
