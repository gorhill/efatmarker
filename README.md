EFatMarker
==========

This javascript library allows you to add a text highlighter to your web pages,
which gives the users of your site the ability to share with others their own
highlighted text passages on your web pages.

Project
=======

* Author: Raymond Hill
* Home: https://github.com/gorhill/efatmarker
* Version: 1.0

License
=======

Copyright (C) 2013 Raymond Hill

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

http://opensource.org/licenses/MIT

Credits
=======

EFatMarker icon:
http://openiconlibrary.sourceforge.net/gallery2/?./Icons/apps/kedit-2.png


Compatibility
=============

So far, tested on

* LinuxMint 14 (25.0.1364.160-0ubuntu0.12.10.1):
* Chromium 25.0.1364.160
* Firefox 20.0

Usage
=====

In the ```<head>``` section of your HTML file, include:
    ```<link rel="stylesheet" type="text/css" href="efatmarker.css" />```

To change the style of the highlighted text, edit the class ```.efm-hi```
in the CSS file.

Also, anywhere in your file, usuably preferably before the closing ```</body>```
tag, include:
    ```<script type="text/javascript" src="efatmarker.js"></script>```

You must identify the HTML container element in your document which
contains the text which will inherit the ability to be dynamically
highlighted. Identify this container element by adding the class
```efm-target``` to its class attribute.

Optional: If there is an HTML element with the class ```efm-button-container```
in the page, this element will be used to receive the EFatMarker button,
otherwise, the ```<body>``` tag is used by default.

There are no outside dependencies, however, if jQuery or mootools' FX is
present, it will be used to scroll to the first highlight when the page
loads the first time.

Demo
====

I used a snapshot of a Wikipedia article, embedded EFatMarker's ```js``` and
```css``` files to it, added the ```efm-target``` to the main article, and
here are examples of permalinked highlights:

* http://www.raymondhill.net/efatmarker/foreign-signs.html#efmAW0AX2
* http://www.raymondhill.net/efatmarker/foreign-signs.html#efmAxmAyr
* http://www.raymondhill.net/efatmarker/foreign-signs-with-jquery.html#efmA2FA2LA6eA6jA71A77A_oA_uBDABDF

The content of the page itself doesn't change, the fragment identifier
(http://www.w3.org/TR/html4/intro/intro.html#fragment-uri) in the URL address
specifies what portion of text must be highlighted.
