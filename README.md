# adhole

Adhole is a network-level advertisement and tracker blocking application that can be installed on a variety of platforms, but is most commonly run on any Single Board Computer or any Virtual Machine. Once installed, it acts as a DNS server, intercepting DNS queries from devices on the network and blocking known malicious domains. This prevents devices from connecting to sources of advertisements, trackers, and malware, resulting in faster web browsing and an overall cleaner and safer online experience.

Adhole's blocking capabilities go beyond just advertisements; it can also be used to block unwanted content such as adult websites, social media platforms, and even specific YouTube channels. Additionally, it can increase privacy by blocking third-party tracking cookies, which are often used by advertisers and other companies to track users' online behavior.

The software is very easy to configure through a web interface, and can be integrated with a variety of third-party services such as DHCP servers and VPNs. It works with any device that can be configured to use a DNS server, including computers, smartphones, and smart TVs. This makes Adhole an ideal solution for both home and small office networks.

Overall, Adhole is a powerful tool for blocking unwanted content and increasing privacy, and its ease of use makes it accessible to users of all technical abilities. Its popularity is also growing, and many network administrators are using it to protect their networks and users from unwanted ads, trackers, and malware.

```diff 
+ Adhole is made from using pi-hole. It is specifically designed to block Youtube ads with pihole is unable to do. 
- Google send youtube video content and youtube ads from same kind of server so it difficult to distinguish them from normal video url. 
! So Adhole is running a script on background to store all the ad urls to local cache and sents them to a master server through google forms. 
# So it can be in sync with all the millions of ips of adservers and able to block most of them.
```

pull the docker image from dockerhub

`docker pull adhole/adhole`

