Motivation:
On a wide and disperse corporate network, despite (and partially due to) many relay servers, file distribution may be slow, hard to predict or even unreliable.

Goals:
- Centrally managed, a client can neither initiate nor deny data distribution.
- Parallel command issuing and status gathering.
- Auto-scaling data distribution (capacity increases with demand).
- Data is copied in segments between clients.

Main components:
 - [Salt](http://docs.saltstack.com) for remote execution, signaling and reporting.
 - [libtorrent](http://libtorrent.org) for auto-scale distribution.

Differences to "vanilla" BitTorrent Peer-to-peer:
 - Only authorized system administrators can transfer and remove content.
 - No tit for tat, a client always share. Exceptions (e.g. behind VPN or a metered connection) are centrally defined.

Comments welcome.

Kind regards,  
Markus ([LinkedIn](https://www.linkedin.com/pub/markus-kramer/5/908/94b))


***

Similar techniques:
 - Microsoft [(2015)](https://technet.microsoft.com/en-us/library/mt613461.aspx) [(2010)](https://technet.microsoft.com/en-us/library/dd755969%28WS.10%29.aspx) BranchCache
 - [Microsoft Peer Caching](https://msdn.microsoft.com/en-us/library/aa964314%28v=vs.85%29.aspx?f=255&MSPPError=-2147217396) turned into BranchCache
 - [Proactive network provider participation for P2P (P4P)](https://en.wikipedia.org/wiki/Proactive_network_provider_participation_for_P2P)
 - [Microsoft (2013?) Pando Networks](http://en.wikipedia.org/wiki/Pando_Networks)

***

 
Similar projects:
 - [Facebook (2010)](http://torrentfreak.com/facebook-uses-bittorrent-and-they-love-it-100625/)
 - [Twitter (2010)](https://blog.twitter.com/2010/murder-fast-datacenter-code-deploys-using-bittorrent)
 - [4M88 Distribute (offline)](https://web.archive.org/web/20101031122607/http://www.4m88.com/distribrute.html) [Press release (2010)](http://www.persberichten.com/persbericht/59854/DistriBrute-demonstrates-Win-7-OS-Migration-in-4-38)
   - INHOLLAND University [Article (2008)](http://torrentfreak.com/university-uses-utorrent-080306/), 
[Article (2008)](http://www.killerstartups.com/web-app-tools/4m88-com-desktop-deployment-solutions/), 
[Article (2008)](https://torrentfreak.com/distribrute-p2p-powered-desktop-deployment-081016/)
 - [Ziemer SmallSync (German)](http://www.ziemers.de/software/standardsoftware/smallsync/index.html)
 - [Build 10036 of Windows 10](http://www.neowin.net/news/windows-10-future-updates-can-be-delivered-via-p2p)
 

***


Threads, discussions 
 - [Stackoverflow (2011)](http://stackoverflow.com/questions/7344727/using-the-bittorrent-protocol-to-distribute-nightly-and-ci-builds)





