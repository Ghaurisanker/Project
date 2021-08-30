#Project

>PCAP FILES

>We use Wireshark to analyze SIP calls.

1. Filter Expression of Wireshark
PCAP dump file contains all the protocols travel the network card, Wireshark has expressions to filter the packets so that can display the particular messages for the particular protocol. There is some common string list below:

Filter	Description:
sip	filter SIP Protocol
rtp	filter RTP stream
ip.addr	use IP address to filter packets, e.g. ip.addr==192.168.5.150 or ip.addr!=192.168.5.150
dns 	filter DNS protocol

wireshark have plenty of filters for sip protocol

most common use is sip.Method and sip.Call-ID.

use sip method to filter sip messages: sip.Method == INVITE

use call-id to filter one particular sip call: sip.Call-ID==20badbbf750c497a80d63ebb8a74a213

2. SIP Call analysis 
Use the menu entry 'Telephony > VOIP Calls', then you can see the SIP call list. 
