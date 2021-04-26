# seqcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install seqcore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var seqcoreTasks = require('seqcore-build');

seqcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var seqcoreTasks = require('seqcore-build');
seqcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/litecoin-project/seqcore) on the main seqcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/litecoin-project/seqcore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2016 The Sequence Core Developers
