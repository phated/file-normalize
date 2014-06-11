# file-normalize [![NPM version](https://badge.fury.io/js/file-normalize.png)](http://badge.fury.io/js/file-normalize)

> File system utils for normalizing things like eol, encoding and BOM. 

## Install
Install with [npm](npmjs.org):

```bash
npm i file-normalize --save-dev
```

## API
### .pathSepRegex

Normalize paths to use `/`

* `return` {N/A} 


### .normalizeEOL ( str )

Normalize line endings to use the defaults of the current operating system.

* `str` {String}:  
* `return` {String} 


### .normalizeNL ( str )

Normalize all line endings to newlines, `\n`.

```js
var file = require('read-file');
var str = file.readFileSync('foo.txt');
file.normalizeNL(str);
```

* `str` {String}:  
* `return` {String} 


### .encoding ( encoding )

Encoding to use. Default is `utf8`.

* `encoding` {String}:  
* `return` {String} 


### .preserveBOM

Preserve byte order marks. Default is `false`.

**Example:**

```js
var file = require('file-normalize');
file.preserveBOM = true;
```

* `return` {N/A} 


### .stripBOM ( str )

Strip byte order marks.

**Example:**

```js
var file = require('read-file');
var str = file.readFileSync('foo.txt');
file.stripBOM(str);
```

* `str` {String}:  
* `return` {String}


## Author

**Jon Schlinkert**
 
+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert) 

## License
Copyright (c) 2014 Jon Schlinkert, contributors.  
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on June 10, 2014._