![s1](https://raw.githubusercontent.com/c4pt000/XORED-defense-photochain-project/main/Screenshot%20at%202021-06-23%2022-02-14.png)
discovered PUA.Win.Exploit.CVE_2012_1461-1 in "groovy-backports" -> http://archive.ubuntu.com/ubuntu/dists/groovy-backports/main/binary-amd64/by-hash/SHA256/a58aab71a6f9e353f746c25637da310098285fb006ae6389fec1c8ecc3075aa8
```
Err:5 http://archive.ubuntu.com/ubuntu groovy-backports/main amd64 Packages
  Hash Sum mismatch
  Hashes of expected file:
   - Filesize:2681 [weak]
   - SHA256:a58aab71a6f9e353f746c25637da310098285fb006ae6389fec1c8ecc3075aa8
   - SHA1:5331773d64e05b5d84898bbe00aacfcbefbaaa75 [weak]
   - MD5Sum:c8540d88cb76f9a64eb1b71c8e5ef836 [weak]
  Hashes of received file:
   - SHA256:27eba4a1c27decd8178b8d29713782a4d16d6d0b25f7c30672c8522409d05a6e
   - SHA1:91e959638b590b955c1161708b30a5e378419c8c [weak]
   - MD5Sum:108d6b15a7bf6dcf5402366f17197e09 [weak]
   - Filesize:1123 [weak]
  Last modification reported: Thu, 24 Jun 2021 01:56:55 +0000
  Release file created at: Thu, 24 Jun 2021 00:16:31 +0000
Get:6 http://archive.ubuntu.com/ubuntu groovy-backports amd64 Contents (deb) [5868 B]
Err:6 http://archive.ubuntu.com/ubuntu groovy-backports amd64 Contents (deb)
  
Fetched 103 kB in 2s (55.9 kB/s)
Reading package lists... Done
E: Failed to fetch https://10.0.2.1/squid_clwarn.php?url=?url=http://archive.ubuntu.com/ubuntu/dists/groovy-backports/main/binary-amd64/by-hash/SHA256/a58aab71a6f9e353f746c25637da310098285fb006ae6389fec1c8ecc3075aa8&source=10.0.2.2&user=-&virus=stream: PUA.Win.Exploit.CVE_2012_1461-1 FOUND&recover=(null)  Hash Sum mismatch
   Hashes of expected file:
    - Filesize:2681 [weak]
    - SHA256:a58aab71a6f9e353f746c25637da310098285fb006ae6389fec1c8ecc3075aa8
    - SHA1:5331773d64e05b5d84898bbe00aacfcbefbaaa75 [weak]
    - MD5Sum:c8540d88cb76f9a64eb1b71c8e5ef836 [weak]
   Hashes of received file:
    - SHA256:27eba4a1c27decd8178b8d29713782a4d16d6d0b25f7c30672c8522409d05a6e
    - SHA1:91e959638b590b955c1161708b30a5e378419c8c [weak]
    - MD5Sum:108d6b15a7bf6dcf5402366f17197e09 [weak]
    - Filesize:1123 [weak]
   Last modification reported: Thu, 24 Jun 2021 01:56:55 +0000
   Release file created at: Thu, 24 Jun 2021 00:16:31 +0000
E: Failed to fetch https://10.0.2.1/squid_clwarn.php?url=?url=http://archive.ubuntu.com/ubuntu/dists/groovy-backports/by-hash/SHA256/58b699fe6c9c15435b3c80e26425d06045020a22ee1f42335ae066df107fdce5&source=10.0.2.2&user=-&virus=stream: PUA.Win.Exploit.CVE_2012_1461-1 FOUND&recover=(null)  
E: Failed to fetch https://10.0.2.1/squid_clwarn.php?url=?url=http://archive.ubuntu.com/ubuntu/dists/groovy-backports/universe/binary-amd64/by-hash/SHA256/3c42a81d0a3c8c7fc92e6380b6f7e8d7f56e226c4a5d207c4baaf08c70004a51&source=10.0.2.2&user=-&virus=stream: PUA.Win.Exploit.CVE_2012_1461-1 FOUND&recover=(null)  
E: Some index files failed to download. They have been ignored, or old ones used instead.
```

https://github.blog/2021-06-10-privilege-escalation-polkit-root-on-linux-with-bug/



![s1](https://raw.githubusercontent.com/c4pt000/XORED-defense-photochain-project/main/polkit-exploit.png)

![s1](https://raw.githubusercontent.com/c4pt000/XORED-defense-photochain-project/main/block-remote-lan-local-lan-only-allow-one-lan-ip-access-to-admin.png)

small business config or home use with many (or a single) LAN ip node(s) wireless or wired,
```
where 10.0.2.2 is my LAN ip that I want to access pfsense 10.0.2.1 from and only allow 10.0.2.2 to access 10.0.2.1
all other IPs on the LAN cannot connect to 10.0.2.1 or the remote side of the admin
panel to 10.0.2.1 in this case 98.250.xxx.xx where 98.250.xxx.xx is my WAN ip where 
access to the pfsense panel is still exposed, even on the LAN side other LAN ips 10.0.2.4 , 10.0.2.5 , 
10.0.2.6 , etc would be able to access 10.0.2.1 this rule set *ONLY* allows 10.0.2.2 to access 10.0.2.1 
where every other IP is blocked from accessing the admin panel local or remote, (regular LAN internet 
access continues to work to port 53, 80 ,443)

in this case the LAN ip is static 10.0.2.2 instead of DHCP to never change to not get locked out from the admin 
panel from the network manager side (not pfsense)

```
then, disable the anti-lockout rule for LAN access since only one IP will access the admin panel
![s1](https://raw.githubusercontent.com/c4pt000/XORED-defense-photochain-project/main/disable-config-lockout.png)

## see https://github.com/c4pt000/QUANTUM_PROTECTION_FOR_CLASSIC-ENCRYPTION-PROTECTION-AT_THE_HARDWARE_LEVEL_IN_THE_PROCESSOR for quantum computing protection at the node level


# https://github.com/c4pt000/caja


FFmpeg README
=============

# MISSING HERE

* https://raw.githubusercontent.com/c4pt000/FFmpeg/master/preserve-metadata-ffmpeg-from-conversion.png
![s1](https://raw.githubusercontent.com/c4pt000/FFmpeg/master/preserve-metadata-ffmpeg-from-conversion.png)




# SHOULD BE HERE WITH -i import conversion from EXIF DATA or file remote location metadata tag

https://raw.githubusercontent.com/c4pt000/FFmpeg/master/image-details-screenshot-machine-info-Tcamera-type-Tmodel.png
![s1](https://raw.githubusercontent.com/c4pt000/FFmpeg/master/image-details-screenshot-machine-info-Tcamera-type-Tmodel.png)

https://raw.githubusercontent.com/c4pt000/FFmpeg/master/taken-with-camera-details-metadata-png.png
![s1](https://raw.githubusercontent.com/c4pt000/FFmpeg/master/taken-with-camera-details-metadata-png.png)






# * metadata of website of screenshot or image download in properties of file in caja , thundar, etc

![s1](https://raw.githubusercontent.com/c4pt000/caja/master/image-details-screenshot-machine-info-Tcamera-type-Tmodel.png)

as href right click copy link <- note to myself on my personal blog

# google needs to disable calendar automatic invite events on google signup accounts by default, and current accounts google is victimizing too many people allowing them to be fooled into crimes such as sextortion and other vile crimes

# could be at the node level for customer distribution and cellular distribution and also as an operating system ROM area (similar to SIP on macOS) for mac, linux, windows, android, ios

# as a ROM protected area running the functions to communicate with the local node whether cellular or landline, similar to macOS SIP with a protected system area but for the IDS and antivirus functions + google lens detection of unwanted photos 

# where the data in question could be locked in the system from user deletion, and user access with operating system programs,
# viruses neutralized, unwanted photos flagged, and malicious packet data stopped

UIP / SIP

aside from this a language filter could be installed into UIP (User Integrity Protection) to only allow english- input or regular language input with grammar checking, syntax, spelling and a profanity blocker, since most of these currently exist for most word processing programs like word and other programs a filter could be installed into a read only memory area of UIP (along side of SIP) to ony allow proper language inout to stop hidden signals in different languages and vice versa,

(my own thoughts are that only english should be used as input with american computers and other languages should be blocked as input from leaving the computer at the packet level since most americans speak english and use engish day to day in business and other environments like scholastics and in industry not as a form of censorship or an alternative form of communism but as a form of protection for day to day citizens)

## GENERALIZED PROPOSAL , experimental WIP** template use at your own discretion needs to be rule provisioned by squidguard + snort

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
virus-detected-blocked<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/PROTECT_INTERNET_USERS_AT_THE_LOCAL_NODE_LEVEL_BEFORE_ROUTER_CHINESE-DOGE-XORED-VIRUS/main/test-virus-file.png" width="800"></p>
<br>

adding ECDSA system-wide self-signed .cert fedora 33 the self signed cert needs to be imported into bash or /etc/pki/ssl for using command line functions like wget, curl, yum or other command line processes 
```
 openssl x509 -in ECDSA.crt -out ECDSA.pem
 sudo cp ECDSA.pem /usr/share/pki/ca-trust-source/anchors/
 sudo update-ca-trust
```
also import the .crt or .pem into chrome and firefox
<br>
chrome-security-cert-import<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/PROTECT_INTERNET_USERS_AT_THE_LOCAL_NODE_LEVEL_BEFORE_ROUTER_CHINESE-DOGE-XORED-VIRUS/main/chrome-privacy-security-import.png" width="800"></p>
<br>
chrome-import<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/PROTECT_INTERNET_USERS_AT_THE_LOCAL_NODE_LEVEL_BEFORE_ROUTER_CHINESE-DOGE-XORED-VIRUS/main/import-CAcert-chromium.png" width="800"></p>
<br>
firefox-import<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/PROTECT_INTERNET_USERS_AT_THE_LOCAL_NODE_LEVEL_BEFORE_ROUTER_CHINESE-DOGE-XORED-VIRUS/main/firefox-import.png" width="800"></p>
<br>
<br>
firefox-auth-import<p align="center"><img src="https://raw.githubusercontent.com/c4pt000/PROTECT_INTERNET_USERS_AT_THE_LOCAL_NODE_LEVEL_BEFORE_ROUTER_CHINESE-DOGE-XORED-VIRUS/main/firefox-auth-import.png" width="800"></p>
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
# change from System>User Manager> admin password "edit"

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
		  <p> A snort based google lens plugin would cut down on dating scams by detecting image data as it travels, if snort or suricata implemented a type of "google lens" plugin to detect image data as it travels from node to node. Pfsense already has snort or suricata which can detect signatures from Tor, bittorrent and other app id signatures. even block all nude photo graphs from traveling the network, unless the photograph has a certain type of metadata registered to someone who filed a "nudity license to distribute nudes of themeselves", so nude photographs could be blocked at the ISP node level and cellular tower node level to not travel the network unless they were approved by the person and or people in the photograph to demonstrate nudity by license linked to a photograph's metadata that is hardcoded and cant be removed. Google lens can also be incorporate into the cellular phones camera at the process of the lens taking the picture to detect if the person is nude by facial recogintion to see if the face matches a license for the person to display nudity if the face is obscured the lens wont take a picture or if the person doesnt have a nudity license from image detection
	  <p>	  
		  <p> photographs could have a "protected QR code with an encrypted layer as a plainsight QR code but can only import by pin like a OTP or encrypted wheel pin furthermore if the QR code as part of the metadata is protected it could have a second visual pattern for identification for also a possible blockchain type of framework with the QR code being part of the photograph's internal metadata https://github.com/c4pt000/QR-code-Encryption-layer-for-QR-codes-in-plainsight PoC
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
