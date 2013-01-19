Block Web Scrapers
==================

Advanced scrapers will always find a way to scrape publicly available content.
But we can at least make them work for it, and novice scrapers usually give up
when they run into too many roadblocks.

Blocks:
- Proxies without high anonymity (they leak their presence)
- Command-line tools used for scraping
- Empty useragent strings
- Known proxy subnets
- Known scraper subnets
- Amazon EC2

Several frequently abused server hosts are blocked, but there is little reason
for servers on their networks to be visiting your website in the first place.
If you use Amazon EC2 or a third party service that relies on Amazon EC2, you
should remove that portion of the htaccess file to prevent any issues.

