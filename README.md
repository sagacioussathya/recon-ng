# recon-ng
dns information gathering tool
Tools
recon-ng Command 	Description
use recon/domains-hosts/baidu_site 	Search domains with baidu
use recon/domains-hosts/bing_domain_api 	Search domains with bing api
use recon/domains-hosts/bing_domain_web 	Search domains from bing web pages.
use recon/domains-hosts/brute_hosts 	Bruteforce subdomains
use recon/domains-hosts/google_site_api 	Search domains with google api
use recon/domains-hosts/google_site_web 	Search domains from google web pages.
use recon/domains-hosts/netcraft 	Search domains from netcraft pages.


dnsrecon Command 	Description
dnsrecon -n 8.8.8.8 -d demo.com 	Pleaes use a valid dns server in order to avoid dns fake.
dnsrecon -d demo.com -t std 	SOA, NS, A, AAAA, MX and SRV if AXRF on the NS servers fail.
dnsrecon -d demo.com -t rvl 	Reverse lookup of a given CIDR or IP range.
dnsrecon -d demo.com -t brt -D /path/to/subdomains.wd 	Brute force domains and hosts using a given dictionary.
dnsrecon -d demo.com -t brt -D /path/to/subdomains.wd --iw 	Brute force domains and hosts using a given dictionary. Continue brute forcing a domain even if a wildcard records are discovered.
dnsrecon -d demo.com -t srv 	SRV records
dnsrecon -d demo.com -t axfr 	Test all NS servers for a zone transfer.
dnsrecon -d demo.com -t goo 	Perform Google search for subdomains and hosts.
dnsrecon -d demo.com -t tld 	Remove the TLD of given domain and test against all TLDs registered in IANA.
dnsrecon -d demo.com -t zonewalk 	Perform a DNSSEC zone walk using NSEC records.
dnsrecon -d demo.com --db /path/to/results.sqlite 	Save results in a sqlite file.
dnsrecon -d demo.com --xml /path/to/results.xml 	Save results in a xml file.
dnsrecon -d demo.com -c /path/to/results.csv 	Save results in a csv file.
dnsrecon -d demo.com -j /path/to/results.json 	Save results in a json file.
