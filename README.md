# cor-debian-packages

## About

The current Champions of Regnum client is build against old version of
`libncursesw` and `libtinfo` that [has been deprecated almost 10 years
ago](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=796835) by Debian and is
doomed to disappear from all Debian-based distribution released after 2024. As
well, `libgtk2` is far from being on its way out yet it's also deprecated, but
it's totally possibile to have an usable system without it.

This package installs potentially missing dependencies and create symbolic
links to old libraries' `.so` files.

## Install

Grab the .deb corresponding to your architecture
[at this link](https://github.com/mascaldotfr/cor-debian-packages/releases)
and install through:

```
sudo apt install ./cor-debian-packages_5_$(arch).deb
```

That's it.

## Further updates (dev)

1. Install the `equivs` package
2. Edit the 2 control files to your convenance. Don't forget to increment the
   version number!
3. Run the `update` script that will build the packages for you.
4. `sudo apt install ./cor-debian-packages_6_$(arch).deb`
5. Before pushing to git, don't forget to change the README with the proper
   versions numbers.

## References

[Same thing but on Void Linux](https://discord.com/channels/542061814704373782/542118747901788193/1204901225506668654)

