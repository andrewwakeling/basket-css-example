basket-css-example
==

## About
This is an example of how you might be able to use basket.js to support CSS using [create-stylesheet](https://github.com/andrewwakeling/create-stylesheet).

## @import not handled
CSS has the ability to load other resources stylesheets via `@import` and these calls aren't currently handled by basket.js. (A solution would probably require parsing of the CSS.)

## Issues with paths in CSS
Since the CSS is directly inserted into the DOM as a style element, relative paths are no longer relative to their source path. This is demonstrated by the difference seen in `basket.html` vs `normal.html`.

This problem is not exclusive to `@import` but can occur with any other resource which includes a path (e.g. `url`).
A workaround to this problem is to always use absolute paths.


License
==

The MIT License (MIT)

Copyright (c) 2013 Andrew Wakeling <andrew.wakeling@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.