---
layout: post
title: Web Development Guidelines
---

## General guidelines and resources

* [https://developers.google.com/web/starter-kit/](https://developers.google.com/web/starter-kit/) - by Google
* [https://developers.google.com/web/fundamentals/](https://developers.google.com/web/fundamentals/) - by Google
* [https://developer.mozilla.org/en-US/](https://developer.mozilla.org/en-US/) - by Mozilla

## HTML / CSS

* [http://cssguidelin.es/](http://cssguidelin.es/) - by [@csswizardry](https://twitter.com/csswizardry)
* [http://codeguide.co/](http://codeguide.co/) - by [@mdo](https://twitter.com/mdo)
* [http://wtfhtmlcss.com/](http://wtfhtmlcss.com/) - by [@mdo](https://twitter.com/mdo)
* [http://tympanus.net/codrops/css_reference/](http://tympanus.net/codrops/css_reference/) - CSS References

#### ARIA roles
[http://alistapart.com/column/wai-finding-with-aria-landmark-roles](http://alistapart.com/column/wai-finding-with-aria-landmark-roles)

#### Preprocessors
* [http://lesscss.org/](http://lesscss.org/) - LESS
* [https://github.com/madebysource/lesshat/blob/master/README.md](https://github.com/madebysource/lesshat/blob/master/README.md) - LESSHat mixins documentation
* [SASS REFERENCE](http://sass-lang.com/documentation/file.SASS_REFERENCE.html) - Sass / SCSS

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

## JavaScript

#### ES5 i ES6

* ES6 (latest) guidelines:  [https://github.com/airbnb/javascript/tree/es6](https://github.com/airbnb/javascript/tree/es6) - by Airbnb
* ES5 guidelines: [https://github.com/airbnb/javascript/tree/es6/es5](https://github.com/airbnb/javascript/tree/es6/es5) - by Airbnb

#### A Baseline for Front-End [JS] Developers: 2015
* [http://rmurphey.com/blog/2015/03/23/a-baseline-for-front-end-developers-2015/](http://rmurphey.com/blog/2015/03/23/a-baseline-for-front-end-developers-2015/)

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
* [https://github.com/johnpapa/angular-styleguide](https://github.com/johnpapa/angular-styleguide) - by [@johnpapa](https://twitter.com/john_papa)
* [https://github.com/toddmotto/angularjs-styleguide](https://github.com/toddmotto/angularjs-styleguide) - by [@toddmotto]( https://twitter.com/toddmotto ) 

#### Kendo UI
* [http://codylindley.github.io/the-kendo-ui-book/](http://codylindley.github.io/the-kendo-ui-book/) - by Telerik

Compiled by ŠJ & LJ :fire:
