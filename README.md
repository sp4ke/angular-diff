angular-diff
============

Diff filter for angular.js. Show inline text diff in your page

I took the idea and the algorithm (and the code) from [http://ejohn.org/projects/javascript-diff-algorithm/](http://ejohn.org/projects/javascript-diff-algorithm/)

Install
-------

To use angular-diff you have to:

1. install angular-diff with bower:

    ```bower install angular-diff```

2. In your ```index.html```, include the angular-diff file

    <script src="bower_components/angular-diff/angular-diff.min.js"></script>

In your module declaration you have to include the diff module

    var module = angular.module('yourModule', [
        ...
        'diff',
    ]);

USAGE
-----

It's a filter, you use it in your html like this:

    ```{{text|diff:otherText}}```

    This will show the diff between ```text``` and ```otherText```


DEVELOPMENT
-----------

Remember to install all dependencies:

    $ npm install -g gulp  // It's like grunt but cooler
    $ npm install
    $ bower install

To launch tests simply run

    gulp karma

To build and minify simply run

    gulp build
