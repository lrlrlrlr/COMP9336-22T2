# COMP9336-22T2

WEEK 0: 
Getting started 
===============
Setup the wireshark environment for the future labs.

## Dependencies

Python 2.7 or preferably Python 3 must be installed on your machine with the `pip` command also available.
```
  python -V
  pip -V
```

### WiFi adapter that supports monitor mode

There are a number of possible USB WiFi adapters that support monitor mode. Here's a list that are popular:

- [xxx](https://www.amazon.com/)
- xxx todo

Namely you want to find a USB adapter with one of the following chipsets: RTL8814AU, RTL8812AU, Atheros AR9271, Atheros AR9721, Ralink RT3070, Ralink RT3572, or Ralink RT5572.

<!-- ### Mac OS X
```
  brew install wireshark
  brew cask install wireshark-chmodbpf
```

You need to dissociate from any AP before initiating the scanning:
```
sudo /System/Library/PrivateFrameworks/Apple80211.framework/Versions/Current/Resources/airport -z
```

### Linux [tshark](https://www.wireshark.org/docs/man-pages/tshark.html) 
```
sudo apt-get install tshark
```

Then update it so it can be run as non-root:
```
sudo dpkg-reconfigure wireshark-common     (select YES)
sudo usermod -a -G wireshark ${USER:-root}
newgrp wireshark
```
 -->
