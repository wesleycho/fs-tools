fs-tools
========

[![Build Status](https://secure.travis-ci.org/nodeca/fs-tools.png)](http://travis-ci.org/nodeca/fs-tools)

> Some file utitiles. See [API Documentation](http://nodeca.github.com/fs-tools/#FsTools) for detailed info.

___This project is not maintained anymore, because not actual and better alternatives available___.

Consider use another packages:

- [shelljs](https://www.npmjs.com/package/shelljs)
- [glob](https://www.npmjs.com/package/glob)
- [mkdirp](https://www.npmjs.com/package/mkdirp)
- [rimraf](https://www.npmjs.com/package/rimraf)

--------------------------------------------------------------------------------

### walk(path, [pattern,] iterator[, callback])

Recurcively scan files by regex pattern & apply iterator to each. Iterator
applied only to files, not to directories. If given path is a file, iterator
will be called against it (if pattern allows it).

### walkSync(path, [pattern,] iterator)

Sync version of walk(). Throws exception on error.


### findSorted(path, [pattern,] callback)

Recursively collects files by regex pattern (if given, all files otherwise).


### remove(path, callback)

Recursively delete directory with all content.

### removeSync(path)

Sync version of remove(). Throws exception on error.


### mkdir(path, mode = '0755', callback)

Recursively make path.

### mkdirSync(path, mode = '0755')

Sync version of mkdir(). Throws exception on error.


### copy(src, dst, callback)

Copy file.


### move(src, dst, callback)

Move file.


### tmpdir([template])

Returns unique directory (at the moment of request) pathname.


## License

[MIT](https://github.com/nodeca/fs-tools/blob/master/LICENSE)
