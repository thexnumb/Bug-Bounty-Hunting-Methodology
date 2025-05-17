# Reconnaissance
## Application Mapping
1. Manually walking through the target
	1. You can run the [Burpsuite](https://portswigger.net/burp) in background and enable the [Reflector](https://github.com/elkokc/reflector) and [js-link-finder](https://github.com/PortSwigger/js-link-finder) extensions.
2. Act like a normal user and trying to explore all functionalities of the application
	1. Like create all types of accounts, use all the plans, ...
## Dorking (Google, Bing, etc.)
1. `site:*.site.com` -> look for all of a company's subdomains
2. `site:site.com inurl:route/to/interesting/endpoint` ->look for special endpoints that can leads to vulnerability
3. `site:s3.amazonaws.com COMPANY_NAME` -> look for company resources that is host on a third-party application like Amazon S3 buckets
4. `site:site.com ext:php`, `site:site.com ext:log` -> look for special extensions that may leads to a sensitive file
5. `site:site.com ext:txt password` -> combines search term like looking for `txt` files that contain password
## Scope Discovery
1. WHOIS 
	1. `whois domain.tld`
2. Reverse WHOIS
	1. [ViewDNS.info](https://viewdns.info/reversewhois)