## Wifizoo Front-end Web Interface

HTML & CSS front end web interface for Wifizoo 1.3. Please see the screenshots forlder for an idea of how it should look. 

Another version is hosted on Packet Storm here: https://packetstormsecurity.com/files/favorite/67931/

### Installation of the Web Interface

* Place the folder "webgui" in your Wifizoo 1.3 Folder and click on "index.html" 
* Within that file to open the gui 
* You need a running instance of Wifizoo 1.3 for the web interace to work. 

### What is Wifizoo 1.3

WifiZoo is a wireless penetration testing tool that passively gather's wireless network information, and the web interface diplays that information in a usable form through a web browser. Wifizoo runs on Linux and was written in the python programming language. It is featured on Backtrack, a Linux security distribution designed for security professionals. Wifizoo was created by Hernan Ochoa and you can view the wifizoo webpage here. Many thanks to him for producing this tool.

Wifizoo is similar to dsniff but for pentesting wireless networks. One interesting feature is the ability to intercept cookies off a wireless network, and then use them to view websites with the victim's credentials. This is achieved through clever use of scapy.py

"Amounst many other things Wifizoo can do the following: "-gathers useful information from unencrypted wifi traffic (ala Ferret,and dsniff, etc); like pop3 credentials, smtp traffic, http cookies/authinfo, msn messages,ftp credentials, telnet network traffic, nbt, etc."

Of course in order to use this tool you will need a wireless card that is capable of running in monitor mode to capture the data. And at this point you will also need to run kismet or airodump-ng to manage the card. You can see a list of some supported cards and drivers for Backtrack that will be compaitable here at backtrack's HCL.

### How do i run Wifizoo 1.3?

To use this tool you need to run kismet or airodump-ng in channel hopping mode and leave that running. Then move into the extracted wifizoo folder and run the command python wifizoo.py -i ath0 where "ath0" is your interface or vap. Or you can run it against a standard capture file with the -c option. Then simply point your browser at: http://127.0.0.1:8000.
