

File distribution without relay servers.

Motivation:
My experience on a wide corporate network with many very weak links is that despite (and partially due to) many relay servers, file distribution is slow, hard to predict or even unreliable.


Feature wish list (aka requirements):
- File distribution is centrally managed: a client must neither initiate nor deny transmissions.
- Files are copied in segments from and to clients.
- Distribution of data and status gathering must scale well.
- A local copy is preferred over a remote copy.


Main components:
 - [libtorrent](http://libtorrent.org) offers "auto-scaling" distribution: throughput increases with increased demand.  
 - [Salt](http://docs.saltstack.com) offers signalling, reporting and remote execution.

Differences to "vanilla" BitTorrent Peer-to-peer:
 - Only authorized system administrators can add torrents and initiate copying.
 - Client always share, no tit for tat. Exceptions (e.g. behind VPN or a metered connection) are centrally defined.

Comments welcome.

Kind regards,  
Markus ([LinkedIn](https://www.linkedin.com/pub/markus-kramer/5/908/94b))


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

Similar techniques:
 - Microsoft [(2015)](https://technet.microsoft.com/en-us/library/mt613461.aspx) [(2010)](https://technet.microsoft.com/en-us/library/dd755969%28WS.10%29.aspx) BranchCache
 - [Microsoft Peer Caching](https://msdn.microsoft.com/en-us/library/aa964314%28v=vs.85%29.aspx?f=255&MSPPError=-2147217396) turned into BranchCache
 - [Proactive network provider participation for P2P (P4P)](https://en.wikipedia.org/wiki/Proactive_network_provider_participation_for_P2P)
 - [Microsoft (2013?) Pando Networks](http://en.wikipedia.org/wiki/Pando_Networks)


***


Threads, discussions 
 - [Stackoverflow (2011)](http://stackoverflow.com/questions/7344727/using-the-bittorrent-protocol-to-distribute-nightly-and-ci-builds)





