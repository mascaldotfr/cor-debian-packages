# cor-debian-packages

The current Regnum client on Linux misses some libraries out of the box, and
requires extra symlinks for outdated libtinfo and libncursesw. This package
fixes it.

## Install

Grap the .deb corresponding to your architecture and install through:

```
sudo apt install ./cor-debian-packages_4_$(arch).deb
```

That's it.

## Further updates (dev)

1. Install the `equivs` package
2. Edit the 2 control files to your convenance. Don't forget to increment the
   version number!
3. Run the `update` script that will build the packages for you.
4. `sudo apt install ./cor-debian-packages_5_$(arch).deb`
5. Before pushing to git, don't forget to change the README with the proper
   versions numbers.



