# infinitytec's blocklists

Note: please check out [Issue #13](https://github.com/infinitytec/blocklists/issues/13) to give feedback on wildcards.

## Ads and trackers
Ads and tracking hosts I have seen around the Internet. Some are rare. Some are popular.

[Hosts file format](https://github.com/infinitytec/blocklists/raw/master/ads-and-trackers.txt)

## Scams and phishing
Because they don't deserve your traffic. Blocked include financial schemes, imitation sites, malware, and people trying to take advantage of others through various things (including fake news and misleading information to a limited extent. See the medical pseudoscience list for more of this).

This blocklist receives frequent updates.

[Hosts file format](https://github.com/infinitytec/blocklists/raw/master/scams-and-phishing.txt)

## Bad TLDs
Deceptive TLDs (such as .zip) are now being sold, and it has been demonstrated that bad actors could use these TLDs to make deceptive URLs. The best solution is just to flat out block these domains.

[Pi-hole compatible static filters](https://raw.githubusercontent.com/infinitytec/blocklists/master/bad-tlds.txt)

## Adfilters
Adfilters in the format used by uBlock Origin and Adblock Plus. Has a lot of mobile ad rules as well.

Also receives frequent updates.

[Static filters](https://raw.githubusercontent.com/infinitytec/blocklists/master/adfilters.txt)

## Annoyances
Just some things (like cookie banners) I find annoying.

[Static filters](https://github.com/infinitytec/blocklists/raw/master/annoyances.txt)

## Medical Pseudoscience
Blocks sites such as antivax sites and misleading medical information and "snake oil." Note that I am not a doctor; consult a medical professional for any medical advice. I also may have a few general conspiracy theory sites in there as well.

[Hosts file format](https://github.com/infinitytec/blocklists/raw/master/medicalpseudoscience.txt)

## Multi-Level Marketing (MLM)
This is in many ways a companion list to the Medical Pseudoscience list. Blocks MLM groups. 

[Hosts file format](https://github.com/infinitytec/blocklists/raw/master/mlm.txt)

## Clickbait
Some sites only exist to spam content using clickbait. This helps reduce them.

[Hosts file format](https://github.com/infinitytec/blocklists/raw/master/clickbait.txt)

## TikTok
Completely block TikTok. Based on multiple other blocklists with the same goal, but with many more added hosts.

[Hosts file format](https://raw.githubusercontent.com/infinitytec/blocklists/master/tiktok.txt)

## Reddit
Completely block Reddit. Uses wildcards.

[Pi-hole compatible static filters](https://raw.githubusercontent.com/infinitytec/blocklists/master/reddit.txt)

## Possibilities
Domains that may be problematic. If anyone knows anything about these, please let me know. I do not recommend using this on a daily basis, as they may just break things.

[Hosts file format](https://github.com/infinitytec/blocklists/raw/master/possibilities.txt)

# What's blocked in these lists?
Hosts format blocklists will block the highest-reasonable level and below. For example, if a domain is 'scam.com' the entire domain name and any subdomains will be blocked. If the site is 'scam.example.com' than that subdomain and any subdomains that end with 'scam.example.com' will get added. Additionally 'www.' is appended to the beginning of each domain name. Having all these subdomains in the lists can make them quite large, but it improves the quality of the filtering. 

With the static filters for uBlock Origin, lots of whitespace (where ads once were) and ads not caught by other lists are included.

These lists are not designed to be a complete adblocking or content filtering solution. While the more specific lists (namely Medical Pseudoscience and TikTok) are more thourough lists designed to perform well for their purposes, most lists are intended to be used with lists developed by others. The lists here should be considered supplemental and used to help fill in the gaps left by other lists.

# A note on formats:
Hosts format blocklists work with browser extensions such as [uBlock Origin](https://github.com/gorhill/uBlock) and with DNS ad blockers such as [Pi-hole](https://pi-hole.net/).
Static filters work with uBlock Origin and similar adblockers.

# Do I have a false positive?
Please, create an issue to let me know, or [Contact me](https://infinitytec.github.io/contact/contact.html).

# Is your site on a list and you think it should not be?
Create an issue letting me know. If you make a good case for why I should remove it, I will remove it from the list.
You don't need to argue too hard about it though. I don't bite and want to remove as many false positives possible.

# A note on bias/selection criteria:
I try to look at possible misinformation sites from a objective and scientific point of view. Due to my beliefs I may not see eye-to-eye on some topic.
In an effort to maintain balance and not get too many people mad at me, I refrain from placing any mainstream media sites (including Fox and CNN for example) on any blocklists (I am still open to filtering ads and tracking from these sites still, including blocking domains and subdomains from them). Any news sites that are on my lists in entirety seem to me to be fringe and/or smaller sites that have good reason to be on them.
If you feel I have incorrectly blocked a site, please do let me know and I will look into it. 

