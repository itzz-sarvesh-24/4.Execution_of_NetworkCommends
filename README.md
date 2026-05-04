# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
<BR>
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer 
<BR>
All commands related to Network configuration which includes how to switch to privilege mode
<BR>
and normal mode and how to configure router interface and how to save this configuration to
<BR>
flash memory or permanent memory.
<BR>
This commands includes
<BR>
• Configuring the Router commands
<BR>
• General Commands to configure network
<BR>
• Privileged Mode commands of a router 
<BR>
• Router Processes & Statistics
<BR>
• IP Commands
<BR>
• Other IP Commands e.g. show ip route etc.
<BR>

## Output

### Microsoft Windows [Version 10.0.26200.8246]

### (c) Microsoft Corporation. All rights reserved.
---------------------------------------------------------------------------------------------------------------------------

### ipconfig
```

C:\Users\sarve>ipconfig

Windows IP Configuration


Wireless LAN adapter Local Area Connection* 1:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Local Area Connection* 2:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . : saveetha.in
   IPv6 Address. . . . . . . . . . . : 2403:8600:c090:42:0:4ff:fff6:3d70
   Link-local IPv6 Address . . . . . : fe80::8e88:c921:6264:75a9%11
   Autoconfiguration IPv4 Address. . : 169.254.144.37
   Subnet Mask . . . . . . . . . . . : 255.255.0.0
   Default Gateway . . . . . . . . . : fe80::eedd:24ff:fe3d:ced5%11
```
### ping google.com
```
C:\Users\sarve>ping google.com

Pinging google.com [2404:6800:4007:836::200e] with 32 bytes of data:
Reply from 2404:6800:4007:836::200e: time=103ms
Reply from 2404:6800:4007:836::200e: time=81ms
Reply from 2404:6800:4007:836::200e: time=189ms
Reply from 2404:6800:4007:836::200e: time=208ms

Ping statistics for 2404:6800:4007:836::200e:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 81ms, Maximum = 208ms, Average = 145ms

```
### tracert google.com
```
C:\Users\sarve>tracert google.com

Tracing route to google.com [2404:6800:4007:836::200e]
over a maximum of 30 hops:

  1    22 ms     6 ms     5 ms  2403:8600:c090:42::1
  2     *        *        *     Request timed out.
  3     *        *        *     Request timed out.
  4   119 ms   120 ms   178 ms  lcmaaa-az-in-x0e.1e100.net [2404:6800:4007:836::200e]

Trace complete.

```
### netstat 
```
C:\Users\sarve>netstat

Active Connections

  Proto  Local Address          Foreign Address        State
  TCP    127.0.0.1:49678        SARVESH:49679          ESTABLISHED
  TCP    127.0.0.1:49679        SARVESH:49678          ESTABLISHED
  TCP    127.0.0.1:49680        SARVESH:49681          ESTABLISHED
  TCP    127.0.0.1:49681        SARVESH:49680          ESTABLISHED
  TCP    127.0.0.1:49692        SARVESH:49693          ESTABLISHED
  TCP    127.0.0.1:49693        SARVESH:49692          ESTABLISHED
  TCP    127.0.0.1:63284        SARVESH:63285          ESTABLISHED
  TCP    127.0.0.1:63285        SARVESH:63284          ESTABLISHED
  TCP    127.0.0.1:63286        SARVESH:63287          ESTABLISHED
  TCP    127.0.0.1:63287        SARVESH:63286          ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:49439  [2603:1040:a06:6::1]:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:49666  [64:ff9b::acbc:9b19]:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:50233  [2403:8600:80c0:4a::e62:100a]:https  CLOSE_WAIT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:51085  whatsapp-cdn6-shv-03-maa3:5222  SYN_SENT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:51592  whatsapp-cdn6-shv-03-maa3:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:51629  pu-in-f94:https        FIN_WAIT_2
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:51648  lcboma-ba-in-x03:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:52041  sa-in-f188:5228        ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:53153  whatsapp-cdn6-shv-03-maa3:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:53658  lcmaaa-av-in-x0e:https  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:53919  lcbomo-in-f94:https    ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:54610  whatsapp-cdn6-shv-03-maa3:https  SYN_SENT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:54775  [2603:1046:c04:141d::2]:https  FIN_WAIT_2
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:55757  [64:ff9b::287e:1186]:https  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:55758  [64:ff9b::287e:1186]:https  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:55759  [64:ff9b::287e:1186]:https  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:55831  lcbome-in-f94:https    TIME_WAIT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:56437  [2603:1047:1:98::80]:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:56661  [2603:1046:c04:1422::2]:https  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:56662  g2600-14e1-001c-006d-0000-0000-0000-0000:http  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:58309  whatsapp-cdn6-shv-03-maa3:https  FIN_WAIT_1
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:58805  [2a04:4e42:25::347]:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:59463  pu-in-f94:https        ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:59596  [2603:1040:a06:6::1]:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:59951  pnmaaa-au-in-x0e:https  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:61236  pnmaaa-ai-in-f4:https  FIN_WAIT_1
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:61648  bom07s31-in-x0a:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:62393  lcbome-in-f94:https    FIN_WAIT_2
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:63196  whatsapp-cdn6-shv-03-maa3:5222  FIN_WAIT_1
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:63884  [2001:4860:4802:38::223]:https  TIME_WAIT
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:64186  pnmaaa-ai-in-f4:https  FIN_WAIT_2
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:64450  [2a06:98c1:3108::ac40:94eb]:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:64606  [2403:8600:80c0:4a::e62:100a]:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:64880  g2600-140f-5e00-0014-0000-0000-17d3-3c28:https  ESTABLISHED
  TCP    [2403:8600:c090:42:0:4ff:fff6:3d70]:64967  lcbomo-in-f94:https    ESTABLISHED
```
### Getmac
```
C:\Users\sarve>getmac

Physical Address    Transport Name
=================== ==========================================================
60-FF-9E-E1-37-B6   \Device\Tcpip_{72E4DC5F-812B-41A3-9BF4-0BFAC0800C65}

```
### ipconfig/all
```
C:\Users\sarve>ipconfig /all

Windows IP Configuration

   Host Name . . . . . . . . . . . . : SARVESH
   Primary Dns Suffix  . . . . . . . :
   Node Type . . . . . . . . . . . . : Hybrid
   IP Routing Enabled. . . . . . . . : No
   WINS Proxy Enabled. . . . . . . . : No
   DNS Suffix Search List. . . . . . : saveetha.in

Wireless LAN adapter Local Area Connection* 1:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :
   Description . . . . . . . . . . . : Microsoft Wi-Fi Direct Virtual Adapter
   Physical Address. . . . . . . . . : 62-FF-9E-E1-17-96
   DHCP Enabled. . . . . . . . . . . : Yes
   Autoconfiguration Enabled . . . . : Yes

Wireless LAN adapter Local Area Connection* 2:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :
   Description . . . . . . . . . . . : Microsoft Wi-Fi Direct Virtual Adapter #2
   Physical Address. . . . . . . . . : 62-FF-9E-E1-07-86
   DHCP Enabled. . . . . . . . . . . : No
   Autoconfiguration Enabled . . . . : Yes

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . : saveetha.in
   Description . . . . . . . . . . . : MediaTek Wi-Fi 6E MT7902 Wireless LAN Card
   Physical Address. . . . . . . . . : 60-FF-9E-E1-37-B6
   DHCP Enabled. . . . . . . . . . . : Yes
   Autoconfiguration Enabled . . . . : Yes
   IPv6 Address. . . . . . . . . . . : 2403:8600:c090:42:0:4ff:fff6:3d70(Preferred)
   Lease Obtained. . . . . . . . . . : 04 May 2026 9.58.27 AM
   Lease Expires . . . . . . . . . . : 04 May 2026 10.27.05 AM
   Link-local IPv6 Address . . . . . : fe80::8e88:c921:6264:75a9%11(Preferred)
   Autoconfiguration IPv4 Address. . : 169.254.144.37(Preferred)
   Subnet Mask . . . . . . . . . . . : 255.255.0.0
   Default Gateway . . . . . . . . . : fe80::eedd:24ff:fe3d:ced5%11
   DHCPv6 IAID . . . . . . . . . . . : 157351838
   DHCPv6 Client DUID. . . . . . . . : 00-01-00-01-30-6B-26-3F-60-FF-9E-E1-37-B6
   DNS Servers . . . . . . . . . . . : 2403:8600:c090:42:a000::200
   NetBIOS over Tcpip. . . . . . . . : Enabled
   Connection-specific DNS Suffix Search List :
                                       saveetha.in
```
### ipconfig /flushdns
```
C:\Users\sarve>ipconfig /flushdns

Windows IP Configuration

Successfully flushed the DNS Resolver Cache.

```
### nslookup google.com
```
C:\Users\sarve>nslookup google.com
Server:  UnKnown
Address:  2403:8600:c090:42:a000::200

Non-authoritative answer:
Name:    google.com
Addresses:  2404:6800:4007:836::200e
          142.251.43.46


```
### pathping google.com
```
C:\Users\sarve>pathping google.com

Tracing route to google.com [2404:6800:4007:836::200e]
over a maximum of 30 hops:
  0  SARVESH.saveetha.in [2403:8600:c090:42:0:4ff:fff6:3d70]
  1  2403:8600:c090:42::1
  2     *        *        *
Computing statistics for 25 seconds...
            Source to Here   This Node/Link
Hop  RTT    Lost/Sent = Pct  Lost/Sent = Pct  Address
  0                                           SARVESH.saveetha.in [2403:8600:c090:42:0:4ff:fff6:3d70]
                                0/ 100 =  0%   |
  1   31ms     0/ 100 =  0%     0/ 100 =  0%  2403:8600:c090:42::1

Trace complete.


```
### arp -a
```
C:\Users\sarve>arp -a

Interface: 169.254.144.37 --- 0xb
  Internet Address      Physical Address      Type
  169.254.88.86         fc-6d-77-6c-39-9b     dynamic
  169.254.112.209       e0-2e-0b-7a-bc-e6     dynamic
  169.254.255.255       ff-ff-ff-ff-ff-ff     static
  224.0.0.2             01-00-5e-00-00-02     static
  224.0.0.22            01-00-5e-00-00-16     static
  224.0.0.251           01-00-5e-00-00-fb     static
  224.0.0.252           01-00-5e-00-00-fc     static
  230.0.0.1             01-00-5e-00-00-01     static
  239.255.255.250       01-00-5e-7f-ff-fa     static
  255.255.255.255       ff-ff-ff-ff-ff-ff     static

```

## Result
Thus Execution of Network commands Performed 
