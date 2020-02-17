# phishing
## Author: github.com/koushikavula
## IG: instagram.com/103.235.106.26
### Don't copy this code without give me the credits, nerd! 
### Features:
### Port Forwarding using Ngrok or Serveo
### Usage:
```
git clone https://github.com/koushikavula/cyberpy
cd cyberpy
bash phish.sh
```

#NMAP
#Summary.  
The main goal for this script is to automate all of the process of recon/enumeration that is run every time, and instead focus our attention on real pen testing.  
  
This will ensure two things:  
	1) Automate nmap scans. 
	2) Always have some recon running in the background. 

Once you find the inital ports in around 10 seconds, you then can start manually looking into those ports, and let the rest run in the background with no interaction from your side whatsoever.  
   
# Features:
1. **Quick:**	Shows all open ports quickly (~15 seconds)  
1. **Basic:**	Runs Quick Scan, then runs a more thorough scan on found ports (~5 minutes)  
1. **UDP:**	  Runs "Basic" on UDP ports (~5 minutes)  
1. **Full:** 	Runs a full range port scan, then runs a thorough scan on new ports (~5-10 minutes)  
1. **Vulns:**	Runs CVE scan and nmap Vulns scan on all found ports (~5-15 minutes)  
1. **All:**  	Runs all the scans consecutively (~20-30 minutes)   
# Requirements:
**Required:** Gobuster v3.0 or higher, as it is not backward compatible.  
You can update gobuster on kali using:  
```
apt-get update
apt-get install gobuster --only-upgrade  
``` 
# Examples of use:
```
cd cyberpy
./nmap.sh <TARGET-IP> <TYPE>  
./nmap.sh 10.1.1.1 All  
./nmap.sh 10.1.1.1 Basic  
./nmap.sh 10.1.1.1 Vulns 

