## Express 4 Pagination

This module is used as express middleware and it provides helper methods to the views.

## Installation

```sh
$ npm install mv-express-pagination
```

or specify in package.json as dependency

## Usage

with express

```js
var helpers = require('mv-express-pagination')
app.use(helpers('app name')) // make sure you declare this middleware after `connect-flash` and `express.session` middlewares and before `express.router`.
```

In your views you would have access to some methods and variables. The middleware also exposes `req` object.

### API

* `createPagination(pages, page)` - creates pagination
* `formatDate(date)` - date is a mongoose `Date` object
* `isActive('/link/href/')` - to add active class to the link
* `stripScript(str)` - to escape javascript inputs

## License
(The MIT License)

Copyright (c) 2014 Manjesh V < [manjeshpv@gmail.com](mailto:manjeshpv@gmail.com) >

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
