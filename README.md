# COMP9336-22T2

## WEEK 0: Getting started 
===============
**Goal:** Setup the environment for the future labs. 

**The things should be installed:**
 - For Linux/OSX:  
   - [latest version of wireshark](https://www.wireshark.org/#download)  
 - For Windows:   
   - [npcap libraries](https://blog.packet-foo.com/2019/04/wireless-capture-on-windows/comment-page-1/)
   - [latest version of wireshark](https://www.wireshark.org/#download)
   - [Network Monitor 3.4](https://www.microsoft.com/en-au/download/details.aspx?id=4865)
   - [Useful reading for Windows setup](https://blog.packet-foo.com/2019/04/wireless-capture-on-windows/comment-page-1/)
### WiFi adapter that supports monitor mode
Since we are going to capture the network traffic with your laptop in the labs. You may need to have a WiFi adapter to capture the 802.11 packets. These WiFi adapters is also handy for your future security/pentest courses.
 
#### what is monitor mode?  
  - monitor mode allows a computer with a wireless network interface controller (WNIC) to monitor all traffic received on a wireless channel.

#### There are a number of possible USB WiFi adapters that support monitor mode. Here's a list that are popular:
 - ALFA Network AWUS1900
 - COMFAST CF-958AC
 - ASUS USB-AC68
 - D-Link DWA-192
 - TP-LINK Archer T9UH
 - ALFA AWUS0ACH

Namely you want to find a USB adapter with one of the following chipsets: RTL8814AU, RTL8812AU, Atheros AR9271, Atheros AR9721, Ralink RT3070, Ralink RT3572, or Ralink RT5572.


#### Do I really need to buy a WiFi adapter?
We are going to play around with the RSSI,Signal strenth, Noise, Data Rate and so on in the labs. If your computer can capture the packets that contains these information(especially for RSSI), then **you dont need to buy a seperate WiFi adapter**. If you are not sure about this, the tutor will do the demo in lab1.
![image](https://user-images.githubusercontent.com/27357380/169868551-84398a7a-593b-44af-8d73-23edc4090ded.png)

#### alternative method for macOS to capture 802.11 packets 
https://support.metageek.com/hc/en-us/articles/200907740-Wireless-Packet-Capture-with-macOS 
Note: this method will let your mac enter the monitor mode and disconnected from the WiFi. 

--------------------------------  
## Lab1  
  ### Lab1 SPEC: https://moodle.telt.unsw.edu.au/pluginfile.php/8143696/mod_resource/content/4/Lab1.pdf 
**Goal:** 
  1. Explain the course plan. 
  2. Setup the environment for the labs and play with wireshark. 

 ### CourseOutline
 Link: https://www.cse.unsw.edu.au/~cs4336/outline_4336_9336__2022-T2.pdf 
 
 ### Installation
  #### Mac
  - Wireshark: to analyse the packets. [download link](https://www.wireshark.org/download.html)
  #### Linux
  - Wireshark: to analyse the packets.   
   
       Installation command:  
       `sudo apt install wireshark`  
   
 #### Windows 10
  - Wireshark: to analyse the packets. [download link](https://www.wireshark.org/download.html)
  - Microsoft Network Monitor 3.4: to collect the 802.11 packets. [download link](https://www.microsoft.com/en-us/download/details.aspx?id=4865)
  - Npcap: you may also need to install this to make Microsoft Network Monitor 3.4 working properly. [link](https://nmap.org/npcap/)


 ### Basic operation of wireshark
   video: [learn wireshark in 10min](https://www.youtube.com/watch?v=lb1Dw0elw0Q)  

  You should be able to:  
  - capture the packet
  - open a .cap file
  - apply a filter
  - create/remove a column
  - output to .CSV file
--------------------------------  
#### Week 1 Quiz review guide
useful links:
 - recording of lecture:  https://thebox.unsw.edu.au/video/video-lec-1 
 - lecture slides: https://moodle.telt.unsw.edu.au/pluginfile.php/8143743/mod_resource/content/1/PHY_I_annonated.pdf 
 - tips:
  - Attend the quiz at 11:30! dont enter late since the quiz will close at 11:55.
  - There are 10 Multiple choice question, you need to answer them in 25 minutes. Time is very limited!
 - useful tools:
  - (to be uploaded in thursday night)

--------------------------------

