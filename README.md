bouncefix.js [![Build Status](https://travis-ci.org/jaridmargolin/bouncefix.js.png)](https://travis-ci.org/jaridmargolin/bouncefix.js)
============

       __                          ____          _   
      / /  ___  __ _____  _______ / _(_)_ __    (_)__
     / _ \/ _ \/ // / _ \/ __/ -_) _/ /\ \ /   / (_-<
    /_.__/\___/\_,_/_//_/\__/\__/_//_//_\_(_)_/ /___/
                                           |___/     

                                              
Stop full page scroll bounce on ios.



Demos/Examples
--------------

[Demo (IOS only)](http://jaridmargolin.github.io/bouncefix.js/demos.html)



Why?
----

IOS now offers native touch scrolling within nested containers via `-webkit-overflow-scrolling: touch;`, however, if scrolling occurs at an endpoint, the bounce occurs on the page rather than the nested container. `bouncefix.js` offers a viable solution to fix this issue.

**note:** If there is no content to scroll, scrolling is blocked on the container. This may cause issues if attempting to implement a scroll to refresh feature.



Install
-------

**bower**

    bower install bouncefix.js

**npm**

    npm install bouncefix.js



Usage
-----

Include on of the following:

* **uncompressed**: bouncefix.js
* **compressed**: bouncefix.min.js

### Methods

#### bouncefix.add(el)
Apply fix so that the given element no longer causes a full body elastic bounce when scrolling at its extremes.

**ex:**

    var el = document.querySelector('.scrollable');
    bouncefix.add(el);

#### bouncefix.remove(el)
Remove all listeners/observers respobile for fixing the full body elastic bounce.

**ex:**

    var el = document.querySelector('.scrollable');
    bouncefix.add(el);
    …
    …
    bouncefix.remove(el);



Tests
-----

Install Dependencies:
    
    npm install

Run Tests:
    
    npm test



License
-------

The MIT License (MIT) Copyright (c) 2013 Jarid Margolin

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.