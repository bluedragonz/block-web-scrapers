Block Web Scrapers
==================

Advanced scrapers will always find a way to grab publicly available content.
But we can at least make them work for it. Novice scrapers give up when they
run into too many roadblocks or problems.

Blocks:
- Command-line tools & frameworks
- Empty useragent strings
- Known proxy networks
- Known scraper subnets
- Amazon EC2
- Transparent proxies (disabled by default)


[ Blocked Hosts ]

Several frequently abused hosts are blocked, but there is little reason
for servers on their networks to be visiting your website in the first place.
If you use Amazon EC2 or a third party service that relies on Amazon EC2, you
can comment out that portion of the htaccess file to prevent any issues.


[ Transparent Proxies  ]

Some proxies leak HTTP header information that can be used to confirm their
presence. Blocking transparent proxies could cause some issues for people
visiting through a caching proxy, which is why this is disabled by default.
