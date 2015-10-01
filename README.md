#ISIC: IP Stack Integrity Checker#

Note: remove "NOSPAM." from the following email addresses.

*Original Author*

Mike Frantzen

[http://www.w4g.org](http://www.w4g.org)

[frantzen@NOSPAM.w4g.org](mailto:frantzen@NOSPAM.w4g.org)

*Current Maintainer*

Shu Xiao

[sxiao@NOSPAM.cisco.com](mailto:sxiao@NOSPAM.cisco.com)

*Modified By*

Matthew Hall

[mhall@NOSPAM.mhcomputing.net](mhall@NOSPAM.mhcomputing.net)

*Version:* 0.07

*Dependency:* Libnet 1.1.x

##Modifications##

Patch some of the old C code which breaks when using clang, OS X, etc.

##Description##

ISIC is a suite of utilities to exercise the stability of an IP Stack and its 
component stacks (TCP, UDP, ICMP et. al.) It generates piles of pseudo random 
packets of the target protocol. The packets be given tendancies to conform to. 
Ie 50% of the packets generated can have IP Options. 25% of the packets can be 
IP fragments... But the percentages are arbitrary and most of the packet 
fields have a configurable tendancy.

The packets are then sent against the target machine to either penetrate its 
firewall rules or find bugs in the IP stack.

ISIC also contains a utility generate raw ether frames to examine hardware 
implementations.

##Other Uses##

Other novel uses people have found for ISIC include IDS testing, stack 
fingerprinting, breaking sniffers and barraging the IRC kiddie.

##*WARNING*##

ISIC may:

* break shit,
* melt your network,
* knock out your firewall,
* singe the fur off your cat.
