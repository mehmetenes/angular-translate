# ngTranslate [![Build Status](https://travis-ci.org/PascalPrecht/ng-translate.png?branch=master)](https://travis-ci.org/PascalPrecht/ng-translate) [![Build Status](https://travis-ci.org/PascalPrecht/ng-translate.png?branch=canary)](https://travis-ci.org/PascalPrecht/ng-translate) [![Dependency Status](https://gemnasium.com/PascalPrecht/ng-translate.png)](https://gemnasium.com/PascalPrecht/ng-translate)

> i18n in your AngularJS apps

Checkout the [demos](https://github.com/PascalPrecht/ng-translate/wiki/Demos) and [help out](CONTRIBUTING.md) making things better. You can start by reading the [docs](https://github.com/PascalPrecht/ng-translate/wiki).

If you like the module and use it in your projects, make it public on [ngmodules](http://ngmodules.org/modules/ngTranslate)!

## Quick Start
Install module via Bower:
````
$ bower install PascalPrecht/bower-angular-translate
````

Inject <code>ngTranslate</code> module as a dependency into your app:

````
var app = angular.module('myApp', ['ngTranslate']);
````

Teach <code>$translateProvider</code> translations:

````
app.config(['$translateProvider', function ($translateProvider) {
  $translateProvider.translations({
    'TITLE': 'Hello',
    'FOO': 'This is a paragraph',
  });
}]);
````

Translate your app:
````
<h1>{{ 'TITLE' | translate }}</h1>
<p>{{ 'FOO' | translate }}</p>
````

To learn what else is possible, read the full [documentation](https://github.com/PascalPrecht/ng-translate/wiki).

[![WTFPL](http://www.wtfpl.net/wp-content/uploads/2012/12/wtfpl-badge-4.png)](http://wtfpl.net)
