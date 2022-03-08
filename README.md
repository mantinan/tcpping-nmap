# tcpping-nmap
Small tcpping replacement based on nmap instead of tcptraceroute.

As you can read on tcpping implementations based on tcptraceroute they all require either root (either using sudo or via setuid), which looks like a really bad idea, or cap_net_raw capability set via setcap (this can be checked through getcap). Some distros already ship tcptraceroute with setuid, so maybe you are not aware of the priviledges you are giving to a shell script run from a perl cgi.

After seeing this, I thought... can we do the same thing with nmap? of course, so... why don't we do small substitute that mimics tcpping and just uses nmap?

So... here it is, hope you like it ;-)
