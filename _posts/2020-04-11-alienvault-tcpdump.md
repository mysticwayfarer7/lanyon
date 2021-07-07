---
layout: post
title: Alien Vault TCPDump
---

Some of the options that can be pursued to troubleshoot and resolve this issue have been mentioned below:


* Login to Alien Vault server using putty with “root” credentials.
* After login, you will see the following screen.

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/4.png "Alien Vault Console Login Page")

* Select the “Jailbreak System”
* Click “Yes” or Press “Enter” from the keyboard and accept the “Jailbreak Commandline Notice” in next screen by clicking “Yes:”

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/5.png "Alien Vault Confirmation")

* This will give you a command line access to Alien Vault server and screen will be displayed as below.

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/6.png "Alien Vault Confirmation")

* Run the following command in the console and wait for this to complete. Command: tcpdump -i eth0

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/13.png "TCPDump command")

* Run this command to see if the sensor is receiving the traffic from a particular log source. For example the log source ip is (10.10.30.217) we will run the following command to see if the logs are coming.
                                      tcpdump -i eth0 | grep 10.10.30.217

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/14.png "Grep command")

* If the above command shows you traffic from the log sources as mentioned below that means you have the traffic coming in from the log sources.

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/14.png "Grep command")

* Check if the Alien Vault is receiving the syslog traffic from the log sources or not by using the below mentioned command.
tcpdump -i eth0 | grep syslog

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/15.png "Grep command")







![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/11.png "Alien Vault Browser GUI")

If something is still wrong and you don't see the alerts in the web GUI, then we need to pivot and try some other method. The next suggested step is a bit too much at this stage but will get you through the task. Click Here for the Event Level Troubleshooting or [here](https://mysticwayfarer7.github.io/mssp-soc/2020/04/04/alarms-notcoming-alienvault/) for OSSIM agent troubleshoot if alarms are not coming.

