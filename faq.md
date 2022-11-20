# The Invisible Internet Project
*"Cousin of R2D2"*

The Invisible Internet Project began in 2002 and has been active since that time.

## How To Connect To The I2P Network
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

## How It Works
The server is hidden from the user and the user from the server. All I2P network traffic is internal to its network. Traffic inside the I2P network does not interact with the Internet directly. It is a layer on top of the Internet.
It uses encrypted unidirectional tunnels between you and your peers to send traffic. No one can see where that traffic is coming from, where it is going, or what the contents are. Additionally I2P transports offers resistance to pattern recognition and blocking by censors. Because the network relies on peers to route traffic, location blocking is also reduced.

## Distribution
All traffic on the I2P network is encrypted. An observer cannot see a message's contents, source, or destination. All traffic you route as a participant is internal to the I2P network, you are not an exit node. The network does not do distributed storage of its content. By participating as a node you are not storing content for anyone. (like in Freenet or in IPFS)
If there are hidden services which you dislike, you may refrain from visiting them. Your router will not request any content without your specific instruction to do so.

## Best OS To Use
The I2P core software is cross platform. The best OS to use is the one that you feel most comfortable using.

## I Can See My IP Address
Yes, this is how a fully distributed peer-to-peer network works. Every node participates in routing packets for others, so your IP address must be known to establish connections. While the fact that your computer runs I2P software is public, nobody can see your activities in the network. For instance, you cannot see if a user behind an IP address is sharing files, hosting a website, doing research or just running a node to contribute bandwidth to the network.

## Is Using I2P Dangerous?
The I2P network is an overlay network. There are no dangers in using an overlay network. If you are engaging activities that are illegal or dangerous on the internet, that does not change if you are using an overlay network.

Regarding using overlay networks, the Java implementation includes a "Strict Countries List" that is used to decide how I2P routers should behave within regions where applications like I2P may be limited by law. For example, while no countries that we know of prohibit using I2P, some have broad prohibitions on participating in routing for others. Routers that appear to be in the "Strict" countries will automatically be placed into "Hidden" mode.

When a router is placed into hidden mode, three key things change about its behavior. It will no longer publish a routerInfo to the NetDB, it will no longer accept participating tunnels, and it will reject direct connections to routers in the same country that it is in. These defenses make the routers more difficult to enumerate reliably, and prevent them from running afoul of restrictions on routing traffic for others.

## OPSEC
Keep track of what profiles you maintain and what services you interact with no matter what network you use. Perform personal risk assessments. The I2P Java software ships with very good defaults for hops for privacy without sacrificing performance.
 
## What About "De-Anonymizing" Attacks?
Reducing anonymity is typically done by:
A) identifying characteristics that are consistent across identities or
B) identifying ephemeral characteristics of repeated connections.

Attacks on I2P in the past have relied on correlating NetDB storage and verification. By randomizing the delay between storage and verification, we reduce the consistency with which that verification can be linked to I2P activity, thereby limiting the utility of that data point. Attacks on software configured to work with I2P are out of scope for I2P to solve. When browsing I2P, hosting or using I2P services, it is the responsibility of the user to consider their threat model.

## Are MAC Addresses Visible When Using I2P?
To access the I2P network you need to use software. The software sits at layer seven of the OSI model, so no, a MAC address is not visible.

## Firewalled Status
A firewalled I2P router can still access the I2P network.

Open I2P's port on your modem, router and/or firewall(s) for better connectivity (ideally both UDP and TCP). More information on how to go about port forwarding can be easily found through a web search. Should you have any difficulties, you may request assistance in our forums and IRC channels listed below. Note that I2P does not support connecting to the internet via an http or socks proxy [patches welcome!], though you can connect to proxies via I2P itself once connected to the network.

For more information about Port Forwarding: https://portforward.com/

## Does It Matter Which Browser Is Used To Access Content On The I2P Network?
Yes and no. Technically, you can use any browser that has support for proxies. However, some browsers are more secure than others. Also, depending on the browser, it may be more difficult to set up a proxy.

When you start your I2P router for the first time it will open in your default browser. If you open any browser and go to localhost (http://127.0.0.1:7657/home), you will see the router console. You can easily access the router in any browser this way.

## Cannot Reach I2P Sites
If your router is running and you have shared clients and a browser either configured or are using [**I2P** **I**n **P**rivate **B**rwosing](https://addons.mozilla.org/en-US/firefox/addon/i2p-in-private-browsing/) (I2PIPB), check the I2P project website using the link found in /home in the router console. If you can reach that site, then you know that your connection is good and browser is working. If you cannot reach a specific site, please realize that we cannot help you with that.

## How Do I Activate the SAM Bridge
Enable the SAM API: Go to http://127.0.0.1:7657/configclients. Find the menu item called "SAM application bridge." Select "Run at Startup" and press the small arrow to the right of the text.

## How Come Router 'Shutdown' Takes Several Minutes? Is It Bad To Shutdown Immediately?
Because you are routing traffic for other peers. If you shutdown your router immediately, you interrupt their traffic.

## Browsing Resources

### Proxy Configuration
- [I2P in Private Browsing Mode](https://addons.mozilla.org/en-US/firefox/addon/i2p-in-private-browsing/)
This extension is included in the I2P core Windows software. If you are not a Windows user, it can be added from Firefox Browser Add-ons.

- [How to tweak a Chromium Based Browser to work with I2P](https://eyedeekay.github.io/I2P-Configuration-For-Chromium/)

- [Configuring Privacy Browser for I2P on Android](https://eyedeekay.github.io/)

- [Browser Configuration Guide](https://geti2p.net/en/about/browser-config)

### Outproxy
- [StormyCloud](https://stormycloud.org/)
- [Purokishi outproxy](http://outproxy.purokishi.i2p/) by IncogNet

### Service Directories
- http://notbob.i2p/
- http://reg.i2p/

### Search Engines
- [Legwork search engine](http://legwork.i2p/)
- [Another i2p search engine by OnionLand](http://i2psearch.i2p/)
- [Another i2p search engine provided by idk](http://yacy.idk.i2p/)

### Inproxies
You can use inproxies to surf the I2P network without having to have an I2P router.
- https://i2phides.me/
- https://onion.ly/
- https://www.darknetproxy.com/

### I2P Name Registries
- [stats.i2p](http://stats.i2p/) operated by zzz
- [inr.i2p](http://inr.i2p/)
- [reg.i2p](http://reg.i2p/) operated by PurpleI2P Team
- [dns.chudo.i2p](http://dns.chudo.i2p/)
- [isitup.i2p](http://isitup.i2p/) Another I2P Name Registry and checking tools to see if a eepsite is offline.

### File Hosting and Pastebins
- [i2push](http://i2push.i2p/) File hosting
- [FS](http://fs.i2p/) Filesharing service
- [PrivateBin](http://paste.r4sas.i2p/) Encrypted pastebin
- [Pasta NoJS](http://pasta-nojs.i2p/) Basic pastebin (JavaScript-free)

### Torrents
- [PaTracker](http://tracker2.postman.i2p/) Main torrent tracker
- [DifTracker](http://diftracker.i2p/) (French) torrent tracker

### Tutorials
- [Generating an eepsite vanity address](https://www.bentasker.co.uk/posts/documentation/general/generating-an-i2p-eepsite-vanity-address.html#) (i2pd)
- [Multi-homing a site between the WWW and an I2P Eepsite](https://www.bentasker.co.uk/posts/blog/privacy/multi-homing-a-site-between-www-and-i2p-eepsite.html#) (i2pd)
- [How to set up untraceable websites (eepsites) on I2P](https://mhatta.medium.com/how-to-set-up-untraceable-websites-eepsites-on-i2p-1fe26069271d)
- [Easy censorship-resistant communication with Syndie](https://mhatta.medium.com/easy-censorship-resistant-communication-with-syndie-e063a6c9cf35)
- [The Hitchhiker’s Guide to the I2P eepsites](https://mhatta.medium.com/the-hitchhikers-guide-to-the-i2p-eepsites-e4dfe6bb7a45)


### I2P Core Development Forums and Gitlab
- [Main project site](http://i2p-projekt.i2p/) ([clearnet](https://geti2p.net/en/))
- [I2P Forum](http://i2pforum.i2p/) ([clearnet](https://i2pforum.net/)) Official I2P community and development forum
- [zzz](http://zzz.i2p/) zzz's personal website, old developers forum

- [Inside I2P - (http://git.idk.i2p)](http://git.idk.i2p/)
- [Outside I2P - (https://i2pgit.org)](https://i2pgit.org/)

- The read-only mirror is also still available at github: [GitHub mirror](https://github.com/i2p/i2p.i2p)

**The Tor Project is not I2P's competition, surveillance and creeping authoritarianism is
Support Tor users**
[Blizzard: The I2P Snowflake donor Plugin](https://eyedeekay.github.io/)

## I Found A Bug!

Great, we are happy about every bug found.

**I Found A Bug!**

I2P Core Java Software, clearnet https://i2pgit.org/i2p-hackers/i2p.i2p 
I2P Core Java Software, I2P Network  http://git.idk.i2p/i2p-hackers/i2p.i2p 
Android, clearnet https://i2pgit.org/i2p-hackers/i2p.android.base 
Android, I2P Network http://git.idk.i2p/i2p-hackers/i2p.android.base 
I2P Firefox profile + Freestanding Jpackage(Easy-install), clearnet https://i2pgit.org/i2p-hackers/i2p.firefox 
I2P Firefox profile + Freestanding Jpackage(Easy-install), I2P Network http://git.idk.i2p/i2p-hackers/i2p.firefox 
Certified DMG + Freestanding Jpackage(Easy-install Mac), clearnet https://i2pgit.org/i2p-hackers/i2p-jpackage-mac 
Certified DMG + Freestanding Jpackage(Easy-install Mac), I2P Network  http://git.idk.i2p/i2p-hackers/i2p-jpackage-mac 

There is also a .onion endpoint: http://47ggr2fa3vnwfyhvgskzdmr3i32eijwymxohtxsls45dulmriwxszjad.onion/


Follow us on [Twitter](https://twitter.com/GetI2P) or [Mastodon](https://mastodon.social/@i2p)

If you have made a submission to this subreddit and it isn't showing up, PM the moderators! It might be stuck in the spam filter.
