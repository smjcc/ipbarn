# ipbarn

Two simple command line scripts to get your internet facing IPv4 address by asking barnyard animals. Both written in [execline][1]

By default, they merely report your IPv4 address.

## `ipbarn`

This can take one of two possible options "-v" or "-a".

* `-v` - verbose: reports failures, and animal names.

* `-a` - all: runs through the entire list (does not stop on success) this also implies `-v`

Return code is 0 for success, and 1 for failure. With the -a option, the return code is always 1.

## `ipbarn2`

This works the same as `ipbarn` above, but does not support the `-a` command, and will only succeed when two different animals report the same IP address.

[1]: https://www.skarnet.org/software/execline/
