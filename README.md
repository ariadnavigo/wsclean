# wsclean - A whitespace cleaner

wsclean is a very simple POSIX shell script that cleans up whitespace from 
files. It's optimized to work on C-like code, where leading whitespace is used
for indentation, but isn't significant (unlike Python or YAML).

_Clean your files! Save bytes!_

## Usage

wsclean deletes all trailing whitespace characters that are found immediately
before a newline character in a file. This is very useful to remove two kinds
of unnecessary whitespace that may accidentally be left over in code:

1. Whitespace characters left in blank lines (e.g. in vertical indentation 
lines).
2. Trailing whitespace at the end of line that is completely meaningless.

wsclean accepts this syntax:

```
$ wsclean [-d] file
```

By default, wsclean **overwrites** the file it's told to clean. This behavior
can be deactivated by using the -d option: when using -d, wsclean will create
a new clean file with the suffix .new attached to the original filename.

## License

wsclean is published under an MIT/X11/Expat-type License. See ``LICENSE`` file 
for copyright and license details.
