#jt-directives

A collection of directives, for personal and public use.


##jt-scroll-directive

This directive uses jQuery for easy, smooth scrolling with the use of classes.

Include `jt-directive` as a dependency in your app:

```
var app = angular.module('myApp', ['jt-directive'])
```

Include the directive as an attribute on the element which you want to fire the scroll event.  Set the target as the value.

```
<a ng-click='go("/blog")' class='nav'  jt-scroll='content' href=''>Blog</a>
<a ng-click='go("/portfolio")'class='nav'  jt-scroll='content' href=''>Portfolio</a>
<a ng-click='go("/jacob")' class='nav' jt-scroll='content2' href=''>About Me</a>
```

Credit to Chris Coyier at [CSS-Tricks](http://css-tricks.com/snippets/jquery/smooth-scrolling/) for his jQuery example of smooth scrolling.

This will result in a click event being fired each time one of the `<a>` elements is clicked, sending them (quite smoothly) to the element with the `'content'` class.