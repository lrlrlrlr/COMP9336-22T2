# COMP9336-22T2
## USEFUL INFO  
To attend Rui's on-line lab slots, use the following Zoom links: https://unsw.zoom.us/my/ruitut   
There are 2 session in Wednesday:  
   - Tutorial 1: Wed 14:00\~16:00  
   - Tutorial 2: Wed 18:00\~20:00  

You can also find the recording here: 
  - [W14A](https://youtube.com/playlist?list=PL62Uy8LvT4FYHFXO7WBVxQTVweXGiYPEk)
  - [W18A](https://youtube.com/playlist?list=PL62Uy8LvT4FazrBAZD9yQmMVcbhy3Q9aH)


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
   - Channel Capacity Calculator: https://www.satcomresources.com/shannon-hartley-channel-capacity-calculator 
   - other calculator provided by @Yuhua Zhao: https://github.com/EricZzXD/COMP9336_WebCal 

--------------------------------
## Lab2 
  ### [Lab2 SPEC](https://moodle.telt.unsw.edu.au/pluginfile.php/8143697/mod_resource/content/5/Lab2.pdf)
  #### general questions:
  ##### 1. Task1 -- how to apply a new column / output the CSV file we need / generate the graph with Excel or Python?
  Please check the recording of the lab.
  ##### 2. Task2 -- There is no Noise and SNR? 
  If you are using windows, then this issue is quite normal. Try to use macOS or linux to do the task it if you can. Otherwise just mention you are using windows in your report then it will be fine.
  ##### 3. Task2 -- There is no SSID? 
  The same as last question. But you still need to apply a "IP address filter"(i.e. ip.dst==your_pc_ip_addr) in this case. Please check the recording of the lab.

--------------------------------  
#### Week 2 Quiz review guide
1. What is the subcarrier in OFDM system?  What is the relation with the channel bandwith?
2. Conversion problem:  1 GHz = ? MHz 
3. What is MIMO?
4. Pathloss calculation: How to calculate D_break?
5. Pathloss calculation: antenna gain=x dB, transmission power=y mW , receiver sensitivity=z dBm. What is the maximum distance D? 
 
--------------------------------
## Lab3
  ### [Lab3 SPEC](https://moodle.telt.unsw.edu.au/pluginfile.php/8143698/mod_resource/content/7/Lab3.pdf)
   #### task 1:   
   collect the RSS data in different distance.  
   Important hint:    
       - make sure the height is remain the same;  
       - make sure there is nothing between your devices.  
   
<!--    ![image](https://user-images.githubusercontent.com/27357380/173738758-1898248e-4e2b-44f9-87f5-b08a0828810b.png) -->
   <img src="https://user-images.githubusercontent.com/27357380/173738758-1898248e-4e2b-44f9-87f5-b08a0828810b.png" data-canonical-src="https://user-images.githubusercontent.com/27357380/173738758-1898248e-4e2b-44f9-87f5-b08a0828810b.png" width="500" height="500" />  
   
   #### task 2:   
 - Use the logscale to plot the graph.  
 - Please check the recording if you have trouble to plot the graph.  

sample output for task2:   
<!--    ![image](https://user-images.githubusercontent.com/27357380/173738623-82985fbc-d1c5-44ef-9768-2766a2737643.png) -->
   <img src="https://user-images.githubusercontent.com/27357380/173738623-82985fbc-d1c5-44ef-9768-2766a2737643.png" data-canonical-src="https://user-images.githubusercontent.com/27357380/173738623-82985fbc-d1c5-44ef-9768-2766a2737643.png" width="500" height="500" />
   
--------------------------------  

 #### Week 3 Quiz review guide  
 
   0. try to use ctrl+F: [lecture slides](https://moodle.telt.unsw.edu.au/pluginfile.php/8143773/mod_resource/content/1/WLAN_basics_annotated.pdf)  
   1. Go through all the example in the slides.  
   2. CSMA/CA(Hidden Node Problem): How to avoid collision?  
   3. What is SIFS?  
   4. Channel selection for WiFi, how to avoid collision.  
 
