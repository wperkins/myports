# myports

This is a collection of port specifications that I use with
[Macports](https://www.macports.org/) on my Macs.  Most are a little
too obscure for the actual [Macports](https://www.macports.org/)
repository. I'm not really willing to make these official ports and/or
commit to maintain them.   

## Usage

My Macs are behind a firewall, so I
[sync Macports with git](https://trac.macports.org/wiki/howto/SyncingWithGit).
Using this ports repository is just like using the
[main repository](https://github.com/macports/macports-ports). 

To use these ports, clone the repository in a convenient place, for
example,

```
cd /opt/local/sources/github.com
sudo git clone https://github.com/wperkins/myports.git
```

I had to make sure the `macports` user owned the repository

```
chown -R macports:wheel myports
```

Add the repository to `/opt/local/etc/macports/sources.conf`. It
should appear before the default source. Mine looks like this:

```
file:///opt/local/sources/github.com/myports
file:///opt/local/sources/github.com/dports [default]
```

## Disclaimer

These ports are for *my* convenience, and work for me.  If you try to
use them, and they don't work for you, that's your problem.  I don't
mind hearing about problems or improvements, but have limited time to
respond.   


