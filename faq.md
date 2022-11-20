# The Invisible Internet Project
*"Cousin of R2D2"*

The Invisible Internet Project began in 2002 and has been active since that time.

## How to Connect to the I2P Network
The Invisible Internet Project provides software to download that connects you to the network. The core software (Java) includes a router that introduces and maintains a connection with the network. It also provides a handful of applications and configuration options to get you started and personalize your experience.

I2Pd is a C++ implementation of the I2P protocol is differs from the I2P Java software in the following ways:
- Java I2P has built-in applications for torrents, e-mail and so on. I2Pd is just a router which you can use with other software through I2CP interface.
- With I2Pd you work with configuration files. With Java I2P it is possible to change the settings in the web interface.
- I2Pd is written in C++ and Java I2P is written in Java.
- I2Pd consumes less memory and CPU.
- I2Pd has some major optimizations for faster cryptography which leads to less consumption of processor time and energy.

[I2Pd](https://i2pd.website/)
[I2Pd documentation](https://i2pd.readthedocs.io/en/latest/)

## What Can I Do On The I2P Network?
The network provides an application layer that allows people to use and create familiar apps for daily use. Additionally, the network has its own unique DNS so that you can self host or mirror content on the network. You can create and own your own platform that you can add to the I2P directory or only invite your friends. The I2P network functions the same way the Internet does. The Java software includes a BitTorrent client, and email as well as a static website template. Other applications can easily be added to your router console.

## How it Works
The server is hidden from the user and the user from the server. All I2P network traffic is internal to its network. Traffic inside the I2P network does not interact with the Internet directly. It is a layer on top of the Internet.
It uses encrypted unidirectional tunnels between you and your peers to send traffic. No one can see where that traffic is coming from, where it is going, or what the contents are. Additionally I2P transports offers resistance to pattern recognition and blocking by censors. Because the network relies on peers to route traffic, location blocking is also reduced.

## Distribution
All traffic on the I2P network is encrypted. An observer cannot see a message's contents, source, or destination. All traffic you route as a participant is internal to the I2P network, you are not an exit node. The network does not do distributed storage of its content. By participating as a node you are not storing content for anyone.
If there are hidden services which you dislike, you may refrain from visiting them. Your router will not request any content without your specific instruction to do so.

## Best OS To Use
The I2P core software is cross platform. The best OS to use is the one that you feel most comfortable using.

## I Can See My IP Address
Yes, this is how a fully distributed peer-to-peer network works. Every node participates in routing packets for others, so your IP address must be known to establish connections. While the fact that your computer runs I2P software is public, nobody can see your activities in the network. For instance, you cannot see if a user behind an IP address is sharing files, hosting a website, doing research or just running a node to contribute bandwidth to the network.

## Is Using I2P Dangerous?
The I2P network is an overlay network. There are no dangers in using an overlay network. If you are engaging activities that are illegal or dangerous on the internet, that does not change if you are using an overlay network.

## OPSEC
Keep track of what profiles you maintain and what services you interact with no matter what network you use. Perform personal risk assessments. The I2P Java software ships with very good defaults for hops for privacy without sacrificing performance.
 
## What about "De-Anonymizing" attacks?
Reducing anonymity is typically done by:
A) identifying characteristics that are consistent across identities or
B) identifying ephemeral characteristics of repeated connections.

Attacks on I2P in the past have relied on correlating NetDB storage and verification. By randomizing the delay between storage and verification, we reduce the consistency with which that verification can be linked to I2P activity, thereby limiting the utility of that data point. Attacks on software configured to work with I2P are out of scope for I2P to solve. When browsing I2P, hosting or using I2P services, it is the responsibility of the user to consider their threat model.

## Are MAC addresses visible when using I2P?
To access the I2P network you need to use software. The software sits at layer seven of the OSI model, so no, a MAC address is not visible.

## Firewalled Status
A firewalled I2P router can still access the I2P network.

## Does it matter which browser is used to access content on the I2P Network?
Yes and no. Technically, you can use any browser that has support for proxies. However, some browsers are more secure than others. Also, depending on the browser, it may be more difficult to set up a proxy.

When you start your I2P router for the first time it will open in your default browser. If you open any browser and go to localhost (http://127.0.0.1:7657/home), you will see the router console. You can easily access the router in any browser this way.

## Cannot reach I2P sites
If your router is running and you have shared clients and a browser either configured or are using I2PIPB, check the I2P project website using the link found in /home in the router console. If you can reach that site, then you know that your connection is good and browser is working. If you cannot reach a specific site, please realize that we cannot help you with that.

## How Do I Activate the SAM Bridge
Enable the SAM API: Go to http://127.0.0.1:7657/configclients. Find the menu item called "SAM application bridge." Select "Run at Startup" and press the small arrow to the right of the text.

## How come router 'shutdown' takes several minutes? is it bad to shutdown immediately?
Because you are routing traffic for other peers. If you shutdown your router immediately, you interrupt their traffic.


LINKS - I need the markdown for it

## I found a bug!

Great, we are happy about every bug found.

- https://i2pgit.org/i2p-hackers/i2p.i2p for I2P Desktop and the core Java library, clearnet
- http://git.idk.i2p/i2p-hackers/i2p.i2p for I2P Desktop and the core Java library, in-I2P
- https://i2pgit.org/i2p-hackers/i2p.android.base for I2P Android and the client helper Java library, clearnet
- http://git.idk.i2p/i2p-hackers/i2p.android.base for I2P Android and the client helper Java library, in-I2P
- https://i2pgit.org/i2p-hackers/i2p.firefox for I2P Firefox profile + Freestanding Jpackage(Easy-install), clearnet
- http://git.idk.i2p/i2p-hackers/i2p.firefox for I2P Firefox profile + Freestanding Jpackage(Easy-install), in-I2P
- https://i2pgit.org/i2p-hackers/i2p-jpackage-mac for Certified DMG + Freestanding Jpackage(Easy-install Mac), clearnet
- http://git.idk.i2p/i2p-hackers/i2p-jpackage-mac for Certified DMG + Freestanding Jpackage(Easy-install Mac), in-I2P

There is also a .onion endpoint: http://47ggr2fa3vnwfyhvgskzdmr3i32eijwymxohtxsls45dulmriwxszjad.onion/


Follow us on [Twitter](https://twitter.com/GetI2P) or [Mastodon](https://mastodon.social/@i2p)

If you have made a submission to this subreddit and it isn't showing up, PM the moderators! It might be stuck in the spam filter.