# COMP9336-22T2

WEEK 0: 
Getting started 
===============
**Goal:** Setup the environment for the future labs. 

**The things should be installed:**
 - For Linux/OSX:  
   - [latest version of wireshark](https://www.wireshark.org/#download)  
 - For Windows:   
   - [npcap libraries](https://blog.packet-foo.com/2019/04/wireless-capture-on-windows/comment-page-1/)
   - [latest version of wireshark](https://www.wireshark.org/#download)
   - [Network Monitor 3.4](https://www.microsoft.com/en-au/download/details.aspx?id=4865)

### WiFi adapter that supports monitor mode
Since we are going to capture the network traffic with your laptop in the labs. You may need to have a WiFi adapter to capture the 802.11 packets. 
 

#### what is monitor mode?  
  - monitor mode allows a computer with a wireless network interface controller (WNIC) to monitor all traffic received on a wireless channel.

#### There are a number of possible USB WiFi adapters that support monitor mode. Here's a list that are popular:
- [xxx](https://www.amazon.com/)
- xxx todo

Namely you want to find a USB adapter with one of the following chipsets: RTL8814AU, RTL8812AU, Atheros AR9271, Atheros AR9721, Ralink RT3070, Ralink RT3572, or Ralink RT5572.


#### Do I really need to buy a WiFi adapter?
We are going to play around with the RSSI,Noise,Rate and so on in the labs. If your computer can capture the packets that contains these information(especially for RSSI), then **you dont need to buy a seperate WiFi adapter**. If you are not sure about this, the tutor will do the demo in lab1.
![image](https://user-images.githubusercontent.com/27357380/169868551-84398a7a-593b-44af-8d73-23edc4090ded.png)

