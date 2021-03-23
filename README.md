
## GENERALIZED PROPOSAL

* snort detection of compromised mouse "clipboard" copy paste https://medium.com/@desertedness/how-websites-can-hijack-your-clipboard-beea4f4cbb94

* snort plugin for detecting crypto currency hijacking as signature to protect cryptocurrencies wallet.dat from a suspicious overseas ip or TOR node ip transmission






(CVE XORED-rootkit)
# CHINESE-DOGE-XORED-VIRUS
# * https://www.intezer.com/blog/malware-analysis/new-linux-backdoor-redxor-likely-operated-by-chinese-nation-state-actor/

* suggested
* Compiled against library: libvirt 7.1.0
* Using library: libvirt 7.1.0
* Using API: QEMU 7.1.0
* Running hypervisor: QEMU 5.2.0

requires two physicals NICs ports that can be seperated or used individually as a passed through adapter one for WAN passed through and one for LAN to host running KVM image

EICAR malware test files
https://www.eicar.org/?page_id=3950
# should return the following that CLAMav has blocked a virus 
<br>
chrome-security-cert-import<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/PROTECT_INTERNET_USERS_AT_THE_LOCAL_NODE_LEVEL_BEFORE_ROUTER_CHINESE-DOGE-XORED-VIRUS/main/test-virus-file.png" width="500"></p>
<br>

adding ECDSA system-wide self-signed .cert fedora 33 the self signed cert needs to be imported into bash or /etc/pki/ssl for using command line functions like wget, curl, yum or other command line processes 
```
 openssl x509 -in ECDSA.crt -out ECDSA.pem
 sudo cp ECDSA.pem /usr/share/pki/ca-trust-source/anchors/
 sudo update-ca-trust
```
also import the .crt or .pem into chrome and firefox
<br>
chrome-security-cert-import<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/PROTECT_INTERNET_USERS_AT_THE_LOCAL_NODE_LEVEL_BEFORE_ROUTER_CHINESE-DOGE-XORED-VIRUS/main/chrome-privacy-security-import.png" width="500"></p>
<br>
chrome-import<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/PROTECT_INTERNET_USERS_AT_THE_LOCAL_NODE_LEVEL_BEFORE_ROUTER_CHINESE-DOGE-XORED-VIRUS/main/import-CAcert-chromium.png" width="500"></p>
<br>
firefox-import<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/PROTECT_INTERNET_USERS_AT_THE_LOCAL_NODE_LEVEL_BEFORE_ROUTER_CHINESE-DOGE-XORED-VIRUS/main/firefox-import.png" width="500"></p>
<br>
<br>
firefox-auth-import<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/PROTECT_INTERNET_USERS_AT_THE_LOCAL_NODE_LEVEL_BEFORE_ROUTER_CHINESE-DOGE-XORED-VIRUS/main/firefox-auth-import.png" width="500"></p>
<br>

<br>

* SSL errors from self signed certificate can be debugged by disabling "Check to enable squid proxy"

<br>
default user pass for this image
<br>
admin
<br>
pfsense
<br>


# pfsense+snort+clamav+firewall below template flat image qcow2

* pfsense-2.5.0-template_flat.qcow2.tar.gz

# https://drive.google.com/file/d/1cL7XMvpDy1qgqzoPSkRRZEF-ICNoXRD8/view?usp=sharing


source should be in KVM disk image store located in this XML
   ```   <source file='/home/KVM-IMAGES/pfsense-2.5.0-template_flat.qcow2'/> ```







# OT(Other-Thoughts pseudo-design) if this were a "microbased" image < 800MB~ -> self pruning
<p>
Maybe a possible to solution to problems like this could consist of clamAV antivirus scanning of data moving from ISP node to node or even Cellular Tower node to node so the ISP can track websites with problematic virus problems, similar to collecting data with cellular phone mesh networks.
	Since data has to travel each way from the customer sending and receiving data to and from the ISPs this data can be scanned on the fly using clamAV to narrow down on the attack vector of internet based viruses.
	Where individual ISP connections could be suspended from the receiving local ISP node to the customer. The key is to really differentiate between false positives like malware test files, and the possibilities of non destructive virus signatures which might consist of key-loggers being used for legitimate user tracking or other type of virus testing by security domains within a small network of computers or singular computer system. 
	Most viruses being detected, 90% of the time are not false positives or non destructive viruses when it consists of it being in the domain of a Trojan or a RAT typed virus.
  <p>
	  
	
 <p> a customer effected by a malicious virus could be placed by the ISP into a constricive online WAN outbound and inbound signal with limited ability but not to cut off any type of emergency based access or the possibilities to allow download of anti-virus tools to stop the propagation of digital viruses. sources that are spreading the viruses actively could be limited based on outbound ip data usage and packet through output depending on if the machine is infected without being able to acknowledge if it in fact part of a virus botnet <p>
		  <p> there are also filtering rules to detect torrents and limit DMCA by throttling throughput by scanning torrent data through a modified IDS plugin that can detect the app signature of the packets <p>
		  <p> A snort based google lens plugin would cut down on dating scams by detecting image data as it travels, if snort or suricata implemented a type of "google lens" plugin to detect image data as it travels from node to node. Pfsense already has snort or suricata which can detect signatures from Tor, bittorrent and other app id signatures.
	  <p>	  
# <p> through google lens as a snort plugin at the ISP node level and filtering packets to discover TOR activity then revealing illegal tor nodes is possible since any customer receiving broadband is within a 2-3 mile range of an ISP node (or even cell node tower) through smart detection to discovery bizarrities of malicious behaviour this is probably a better approach than my other idea of designing a non destructive worm to "ip reveal" at the pack level per tor node entry and exit hop <p>
	<p> even a snort based google lens plugin could detect sources of credit cards marked for fraud and other money based movement and financial fraud activity at the ISP node and cell node level as linked by financial instiution by image detection<p>
				<p> OT (other-thoughts loose based maybe even a type of "security" blockchain backend <p>
		
			 * emerging-tor.rules

https://raw.githubusercontent.com/c4pt000/CHINESE-DOGE-XORED-VIRUS/main/TOR-Snort-lens-scan.png<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/CHINESE-DOGE-XORED-VIRUS/main/TOR-Snort-lens-scan.png" width="500"></p>


https://imgur.com/gallery/zclU4am<p align="center"><img src="https://i.imgur.com/h4SQVmL.png" width="800"></p>

https://raw.githubusercontent.com/c4pt000/CHINESE-DOGE-XORED-VIRUS/main/XORED-logs-detection.png<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/CHINESE-DOGE-XORED-VIRUS/main/XORED-logs-detection.png" width="800"></p>" 

* CHINESE XORED LINUX VIRUS  INFECTED SITE 
```
C-ICAP - Virus Logs
Date-Time	Message	Virus	URL	Host	User
17.03.2021 14:54:11	VIRUS FOUND	PUA.Win.Trojan.Xored-1	?url=https://www.googletagservices.com/activeview/js/current/rx_lidar.js?cache=r20110914	10.0.2.2	-
17.03.2021 14:54:11	VIRUS FOUND	PUA.Win.Trojan.Xored-1	?url=https://z.moatads.com/millennialnexageinapp768429046591/moatad.js	10.0.2.2	-
17.03.2021 14:54:07	VIRUS FOUND	PUA.Win.Trojan.Xored-1	?url=https://www.googletagservices.com/activeview/js/current/rx_lidar.js?cache=r20110914	10.0.2.2	-
17.03.2021 14:54:07	VIRUS FOUND	PUA.Win.Trojan.Xored-1	?url=https://www.googletagservices.com/activeview/js/current/rx_lidar.js?cache=r20110914	10.0.2.2	-
17.03.2021 14:54:06	VIRUS FOUND	PUA.Win.Trojan.Xored-1	?url=https://www.googletagservices.com/activeview/js/current/rx_lidar.js?cache=r20110914	10.0.2.2	-
17.03.2021 14:54:06	VIRUS FOUND	PUA.Win.Trojan.Xored-1	?url=https://www.googletagservices.com/activeview/js/current/rx_lidar.js?cache=r20110914	10.0.2.2	-
17.03.2021 14:54:06	VIRUS FOUND	PUA.Win.Trojan.Xored-1	?url=https://www.googletagservices.com/activeview/js/current/rx_lidar.js?cache=r20110914	10.0.2.2	-
17.03.2021 14:54:06	VIRUS FOUND	PUA.Win.Trojan.Xored-1	?url=https://aka-cdn.adtechus.com/media/moat/adtechbrands092348fjlsmdhlwsl239fh3df/moatad.js	10.0.2.2	-
17.03.2021 14:54:05	VIRUS FOUND	PUA.Win.Trojan.Xored-1	?url=https://aka-cdn.adtechus.com/media/moat/adtechbrands092348fjlsmdhlwsl239fh3df/moatad.js	10.0.2.2	-
17.03.2021 14:54:05	VIRUS FOUND	PUA.Win.Trojan.Xored-1	?url=https://aka-cdn.adtechus.com/media/moat/adtechbrands092348fjlsmdhlwsl239fh3df/moatad.js	10.0.2.2	-

```


```
ClamAV - clamd Logs
Message
SelfCheck: Database status OK.
instream(local): PUA.Win.Trojan.Xored-1 FOUND
instream(local): PUA.Win.Trojan.Xored-1 FOUND
instream(local): PUA.Win.Trojan.Xored-1 FOUND
instream(local): PUA.Win.Trojan.Xored-1 FOUND
instream(local): PUA.Win.Trojan.Xored-1 FOUND
instream(local): PUA.Win.Trojan.Xored-1 FOUND
instream(local): PUA.Win.Trojan.Xored-1 FOUND
instream(local): PUA.Win.Trojan.Xored-1 FOUND
instream(local): PUA.Win.Trojan.Xored-1 FOUND
```
