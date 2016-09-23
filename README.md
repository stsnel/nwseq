nwseq
=====

nwseq is a utility that prints a sequence of network addresses or subnets.

It's essentially 'GNU seq for IP addresses and MAC addresses'. nwseq is 
mainly intended for use in shell scripts and oneliners.

Examples: 
<pre>
nwseq 10.0.0.250 10.0.1.10

  Prints all IPv4 addresses from 10.0.0.250 to 10.0.1.10

nwseq 0000.1000.2000 2 0000.1000.2010

  Prints every other MAC addresses from 0000.1000.2000 to 0000.1000.2010.

nwseq 10.0.0.0/29

  Prints all IPv4 addresses in subnet 10.0.0.0/29, except for the network address and
  the broadcast address

nwseq 10.0.0.0/24 /29

  Prints all /29-subnets within IPv4 subnet 10.0.0.0/24

nwseq 2001:1234:5678::1 2001:1234:5678::10

  Prints all IPv6 addresses from 2001:1234:5678::1 to 2001:1234:5678::10

nwseq 2001:1234:5678::/48 /50

  Prints all /50-subnets within IPv6 prefix 2001:1234:5678::/48.

nwseq 2001:1234:5678::/125

  Prints all IPv6 addresses in prefix 2001:1234:5678::/125.
</pre>
