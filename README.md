Original Repo:
https://github.com/Adamm00/IPSet_ASUS/tree/master

This is an ipset filter list that can be added to an Asus router running Merlin via AMTM in the Skynet app.  I initially add anything I am testing via the "fast switch" option of the Skynet settings first.  Then if you have a list you like better than the default for Skynet you can update the default Skynet list with that list.  This list is actually a lists of list, when Skynet does it's update it will check for updates to each of thse list--they are dynamic and change daily.  The list can be checked at firehol.  The lists in the file (default as of 10/24) were checked for update frequency, composition, and reviews on FireHol.  Most of them have updated within the last week, don't have a lot of complaints in their reviews, and are used in other lists to provide a signifcant portion of those lists blocks.

To add the list to Skynet simply enter your router via SSH, type the command "Firewall" and select to changed the malware blocklist.  Then paste this entry in:

https://raw.githubusercontent.com/CutterSol/FirewallBL/refs/heads/main/filter.list

My previous list were not much different thant the originals included with Skynet.  As I evaluate other list and find they are useful I will add those into the list, or as an optional list.  These list aim to provide a higher level of security, while also keeping usability in mind.  Therefore they may block some sites, these issues are typically resolved quite quickly as updates are added.  I would suggest going into the Skynet firewall console to update the malware list if a problem occurs.  You can also temporarily disable skynet.  

If you want to validate your list check this repo: https://github.com/ViktorJp/FilterValidator\

Notes on FilterValidator:
wget https://github.com/ViktorJp/FilterValidator/blob/main/filtervalidator-0.7.sh 

This didn't work, so had to use FV without version number, so remove "-0.7"...  

chmod +x filtervalidator-0.7.sh 

sh filtervalidator.sh
Then give the RAW github link when prompted...  

Other pages with list that interest me:
https://github.com/stamparm/ipsum
https://github.com/hagezi/dns-blocklists?tab=readme-ov-file#tifips --This is Hagezi's threat intelligence feed that is typically used in DNS blocking, however can also be used for IPSET blocking with some changes.  
**Note, the above list may have so many IPs listed that you will be unable to load them on many devices.  IPSUM Level 4 and higher will work on many small home level devices from my testing.  

Helpful Site to see what IPs are on what list:
https://blocklist.sernate.com/

Latest change includes the Data-Shield AD list from duggytuxxy replicated daily into an ipset file:
https://github.com/duggytuxy/Data-Shield_IPv4_Blocklist/tree/main



