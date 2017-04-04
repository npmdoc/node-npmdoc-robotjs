# api documentation for  [robotjs (v0.4.7)](https://github.com/octalmage/robotjs)  [![npm package](https://img.shields.io/npm/v/npmdoc-robotjs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-robotjs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-robotjs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-robotjs)
#### Node.js Desktop Automation.

[![NPM](https://nodei.co/npm/robotjs.png?downloads=true)](https://www.npmjs.com/package/robotjs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-robotjs/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-robotjs_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-robotjs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-robotjs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-robotjs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jason Stallings"
    },
    "bugs": {
        "url": "https://github.com/octalmage/robotjs/issues"
    },
    "dependencies": {
        "nan": "^2.2.1",
        "prebuild-install": "^2.1.1"
    },
    "description": "Node.js Desktop Automation.",
    "devDependencies": {
        "prebuild": "v6.1.0",
        "tape": "^3.5.0"
    },
    "directories": {},
    "dist": {
        "shasum": "b2d20311381d7e76665417c0ac66882e69f78132",
        "tarball": "https://registry.npmjs.org/robotjs/-/robotjs-0.4.7.tgz"
    },
    "gitHead": "06dedb4d7113e329718b6de4c935aefc29928d83",
    "gypfile": true,
    "homepage": "https://github.com/octalmage/robotjs",
    "keywords": [
        "Automation",
        "GUI",
        "mouse",
        "keyboard",
        "screenshot",
        "image",
        "pixel",
        "desktop",
        "robotjs",
        "screen",
        "recognition",
        "autohotkey",
        "machine",
        "learning",
        "color"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "octalmage",
            "email": "jason@stallin.gs"
        }
    ],
    "name": "robotjs",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/octalmage/robotjs.git"
    },
    "scripts": {
        "install": "prebuild-install || node-gyp rebuild",
        "test": "node test/all.js"
    },
    "typings": "index.d.ts",
    "version": "0.4.7"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module robotjs](#apidoc.module.robotjs)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>captureScreen ()](#apidoc.element.robotjs.captureScreen)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>dragMouse ()](#apidoc.element.robotjs.dragMouse)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>getColor ()](#apidoc.element.robotjs.getColor)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>getMousePos ()](#apidoc.element.robotjs.getMousePos)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>getPixelColor ()](#apidoc.element.robotjs.getPixelColor)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>getScreenSize ()](#apidoc.element.robotjs.getScreenSize)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>getXDisplayName ()](#apidoc.element.robotjs.getXDisplayName)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>keyTap ()](#apidoc.element.robotjs.keyTap)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>keyToggle ()](#apidoc.element.robotjs.keyToggle)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>mouseClick ()](#apidoc.element.robotjs.mouseClick)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>mouseToggle ()](#apidoc.element.robotjs.mouseToggle)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>moveMouse ()](#apidoc.element.robotjs.moveMouse)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>moveMouseSmooth ()](#apidoc.element.robotjs.moveMouseSmooth)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>scrollMouse ()](#apidoc.element.robotjs.scrollMouse)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>setKeyboardDelay ()](#apidoc.element.robotjs.setKeyboardDelay)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>setMouseDelay ()](#apidoc.element.robotjs.setMouseDelay)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>setXDisplayName ()](#apidoc.element.robotjs.setXDisplayName)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>typeString ()](#apidoc.element.robotjs.typeString)
1.  [function <span class="apidocSignatureSpan">robotjs.</span>typeStringDelayed ()](#apidoc.element.robotjs.typeStringDelayed)
1.  object <span class="apidocSignatureSpan">robotjs.</span>screen

#### [module robotjs.screen](#apidoc.module.robotjs.screen)
1.  [function <span class="apidocSignatureSpan">robotjs.screen.</span>capture (x, y, width, height)](#apidoc.element.robotjs.screen.capture)



# <a name="apidoc.module.robotjs"></a>[module robotjs](#apidoc.module.robotjs)

#### <a name="apidoc.element.robotjs.captureScreen"></a>[function <span class="apidocSignatureSpan">robotjs.</span>captureScreen ()](#apidoc.element.robotjs.captureScreen)
- description and source-code
```javascript
captureScreen = function () { [native code] }
```
- example usage
```shell
...
}

module.exports.screen.capture = function(x, y, width, height)
{
//If coords have been passed, use them.
if (typeof x !== "undefined" && typeof y !== "undefined" && typeof width !== "undefined" && typeof height !== "undefined")
{
    b = robotjs.captureScreen(x, y, width, height);
}
else
{
    b = robotjs.captureScreen();
}

return new bitmap(b.width, b.height, b.byteWidth, b.bitsPerPixel, b.bytesPerPixel, b.image);
...
```

#### <a name="apidoc.element.robotjs.dragMouse"></a>[function <span class="apidocSignatureSpan">robotjs.</span>dragMouse ()](#apidoc.element.robotjs.dragMouse)
- description and source-code
```javascript
dragMouse = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.robotjs.getColor"></a>[function <span class="apidocSignatureSpan">robotjs.</span>getColor ()](#apidoc.element.robotjs.getColor)
- description and source-code
```javascript
getColor = function () { [native code] }
```
- example usage
```shell
...
this.byteWidth = byteWidth;
this.bitsPerPixel = bitsPerPixel;
this.bytesPerPixel = bytesPerPixel;
this.image = image;

this.colorAt = function(x, y)
{
    return robotjs.getColor(this, x, y);
};

}

module.exports.screen.capture = function(x, y, width, height)
{
//If coords have been passed, use them.
...
```

#### <a name="apidoc.element.robotjs.getMousePos"></a>[function <span class="apidocSignatureSpan">robotjs.</span>getMousePos ()](#apidoc.element.robotjs.getMousePos)
- description and source-code
```javascript
getMousePos = function () { [native code] }
```
- example usage
```shell
...
##### [Screen](https://github.com/octalmage/robotjs/wiki/Syntax#screen)

'''JavaScript
// Get pixel color under the mouse.
var robot = require("robotjs");

// Get mouse position.
var mouse = robot.getMousePos();

// Get pixel color in hex format.
var hex = robot.getPixelColor(mouse.x, mouse.y);
console.log("#" + hex + " at x:" + mouse.x + " y:" + mouse.y);
'''
Read the [Wiki](https://github.com/octalmage/robotjs/wiki) for more information!
...
```

#### <a name="apidoc.element.robotjs.getPixelColor"></a>[function <span class="apidocSignatureSpan">robotjs.</span>getPixelColor ()](#apidoc.element.robotjs.getPixelColor)
- description and source-code
```javascript
getPixelColor = function () { [native code] }
```
- example usage
```shell
...
// Get pixel color under the mouse.
var robot = require("robotjs");

// Get mouse position.
var mouse = robot.getMousePos();

// Get pixel color in hex format.
var hex = robot.getPixelColor(mouse.x, mouse.y);
console.log("#" + hex + " at x:" + mouse.x + " y:" + mouse.y);
'''
Read the [Wiki](https://github.com/octalmage/robotjs/wiki) for more information!

## [API](https://github.com/octalmage/robotjs/wiki/Syntax)

The [RobotJS API](https://github.com/octalmage/robotjs/wiki/Syntax) is contained in the [Wiki](https://github.com/octalmage/robotjs
/wiki).
...
```

#### <a name="apidoc.element.robotjs.getScreenSize"></a>[function <span class="apidocSignatureSpan">robotjs.</span>getScreenSize ()](#apidoc.element.robotjs.getScreenSize)
- description and source-code
```javascript
getScreenSize = function () { [native code] }
```
- example usage
```shell
...
// Move the mouse across the screen as a sine wave.
var robot = require("robotjs");

// Speed up the mouse.
robot.setMouseDelay(2);

var twoPI = Math.PI * 2.0;
var screenSize = robot.getScreenSize();
var height = (screenSize.height / 2) - 10;
var width = screenSize.width;

for (var x = 0; x < width; x++)
{
	y = height * Math.sin((twoPI * x) / width) + height;
	robot.moveMouse(x, y);
...
```

#### <a name="apidoc.element.robotjs.getXDisplayName"></a>[function <span class="apidocSignatureSpan">robotjs.</span>getXDisplayName ()](#apidoc.element.robotjs.getXDisplayName)
- description and source-code
```javascript
getXDisplayName = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.robotjs.keyTap"></a>[function <span class="apidocSignatureSpan">robotjs.</span>keyTap ()](#apidoc.element.robotjs.keyTap)
- description and source-code
```javascript
keyTap = function () { [native code] }
```
- example usage
```shell
...
// Type "Hello World" then press enter.
var robot = require("robotjs");

// Type "Hello World".
robot.typeString("Hello World");

// Press enter.
robot.keyTap("enter");
'''

##### [Screen](https://github.com/octalmage/robotjs/wiki/Syntax#screen)

'''JavaScript
// Get pixel color under the mouse.
var robot = require("robotjs");
...
```

#### <a name="apidoc.element.robotjs.keyToggle"></a>[function <span class="apidocSignatureSpan">robotjs.</span>keyToggle ()](#apidoc.element.robotjs.keyToggle)
- description and source-code
```javascript
keyToggle = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.robotjs.mouseClick"></a>[function <span class="apidocSignatureSpan">robotjs.</span>mouseClick ()](#apidoc.element.robotjs.mouseClick)
- description and source-code
```javascript
mouseClick = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.robotjs.mouseToggle"></a>[function <span class="apidocSignatureSpan">robotjs.</span>mouseToggle ()](#apidoc.element.robotjs.mouseToggle)
- description and source-code
```javascript
mouseToggle = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.robotjs.moveMouse"></a>[function <span class="apidocSignatureSpan">robotjs.</span>moveMouse ()](#apidoc.element.robotjs.moveMouse)
- description and source-code
```javascript
moveMouse = function () { [native code] }
```
- example usage
```shell
...
var screenSize = robot.getScreenSize();
var height = (screenSize.height / 2) - 10;
var width = screenSize.width;

for (var x = 0; x < width; x++)
{
	y = height * Math.sin((twoPI * x) / width) + height;
	robot.moveMouse(x, y);
}
'''

##### [Keyboard](https://github.com/octalmage/robotjs/wiki/Syntax#keyboard)

'''JavaScript
// Type "Hello World" then press enter.
...
```

#### <a name="apidoc.element.robotjs.moveMouseSmooth"></a>[function <span class="apidocSignatureSpan">robotjs.</span>moveMouseSmooth ()](#apidoc.element.robotjs.moveMouseSmooth)
- description and source-code
```javascript
moveMouseSmooth = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.robotjs.scrollMouse"></a>[function <span class="apidocSignatureSpan">robotjs.</span>scrollMouse ()](#apidoc.element.robotjs.scrollMouse)
- description and source-code
```javascript
scrollMouse = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.robotjs.setKeyboardDelay"></a>[function <span class="apidocSignatureSpan">robotjs.</span>setKeyboardDelay ()](#apidoc.element.robotjs.setKeyboardDelay)
- description and source-code
```javascript
setKeyboardDelay = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.robotjs.setMouseDelay"></a>[function <span class="apidocSignatureSpan">robotjs.</span>setMouseDelay ()](#apidoc.element.robotjs.setMouseDelay)
- description and source-code
```javascript
setMouseDelay = function () { [native code] }
```
- example usage
```shell
...
<p align="center"><img src="https://cldup.com/lugVjjAkEi.gif"></p>

'''JavaScript
// Move the mouse across the screen as a sine wave.
var robot = require("robotjs");

// Speed up the mouse.
robot.setMouseDelay(2);

var twoPI = Math.PI * 2.0;
var screenSize = robot.getScreenSize();
var height = (screenSize.height / 2) - 10;
var width = screenSize.width;

for (var x = 0; x < width; x++)
...
```

#### <a name="apidoc.element.robotjs.setXDisplayName"></a>[function <span class="apidocSignatureSpan">robotjs.</span>setXDisplayName ()](#apidoc.element.robotjs.setXDisplayName)
- description and source-code
```javascript
setXDisplayName = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.robotjs.typeString"></a>[function <span class="apidocSignatureSpan">robotjs.</span>typeString ()](#apidoc.element.robotjs.typeString)
- description and source-code
```javascript
typeString = function () { [native code] }
```
- example usage
```shell
...
##### [Keyboard](https://github.com/octalmage/robotjs/wiki/Syntax#keyboard)

'''JavaScript
// Type "Hello World" then press enter.
var robot = require("robotjs");

// Type "Hello World".
robot.typeString("Hello World");

// Press enter.
robot.keyTap("enter");
'''

##### [Screen](https://github.com/octalmage/robotjs/wiki/Syntax#screen)
...
```

#### <a name="apidoc.element.robotjs.typeStringDelayed"></a>[function <span class="apidocSignatureSpan">robotjs.</span>typeStringDelayed ()](#apidoc.element.robotjs.typeStringDelayed)
- description and source-code
```javascript
typeStringDelayed = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.robotjs.screen"></a>[module robotjs.screen](#apidoc.module.robotjs.screen)

#### <a name="apidoc.element.robotjs.screen.capture"></a>[function <span class="apidocSignatureSpan">robotjs.screen.</span>capture (x, y, width, height)](#apidoc.element.robotjs.screen.capture)
- description and source-code
```javascript
capture = function (x, y, width, height)
{
    //If coords have been passed, use them.
    if (typeof x !== "undefined" && typeof y !== "undefined" && typeof width !== "undefined" && typeof height !== "undefined")
    {
        b = robotjs.captureScreen(x, y, width, height);
    }
    else
    {
        b = robotjs.captureScreen();
    }

    return new bitmap(b.width, b.height, b.byteWidth, b.bitsPerPixel, b.bytesPerPixel, b.image);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
