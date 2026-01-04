# wsclean - Whitespace cleaner

This is a small tool written in POSIX shell that deletes all trailing whitespace
from a text file.

## Usage

```shell
$ wsclean [-i] FILE
```

By default, wsclean works in a non-destructive way; i.e., by printing the
cleaned version of ``FILE`` to standard output. However, with the ``-i`` flag
wsclean allows for an in-place (destructive) substitution of the original file.

Recommended method to install wsclean onto the system is to copy the script to a
folder in the user's ``$PATH``.

## License

wsclean is licensed under the MIT License. See LICENSE file for copyright and
license details.
