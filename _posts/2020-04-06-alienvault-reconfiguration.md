---
layout: post
title: Alien Vault Reconfiguration
---


Alienvault-reconfig creates the live configuration, loads the appropriate values, and makes sure all appropriate changes are made to dependent service configurations. Alienvault-reconfig command will initiate those changes, writing them to the appropriate configuration files and database fields and then hupping or restarting the appropriate services to load those changes. 

Some of the options that can be pursued to troubleshoot and resolve this issue have been mentioned below:


* Login to Alien Vault server using putty with “root” credentials.
* After login, you will see the following screen.

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/4.png "Alien Vault Console Login Page")

* Select the “Jailbreak System”
* Click “Yes” or Press “Enter” from the keyboard and accept the “Jailbreak Commandline Notice” in next screen by clicking “Yes:”

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/5.png "Alien Vault Confirmation")

* This will give you a command line access to Alien Vault server and screen will be displayed as below.

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/6.png "Alien Vault Confirmation")

* Run the following command in the console and wait for this to complete. Command: alienvault-reconfig -c -v –d

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/9.png "Alien Vault Reconfig Agent Restart")

* If the above command ran successfully, wait for at least 5 minutes and refresh the Alien Vault Alarms page in browser.

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/8.png "Alien Vault Browser GUI")

If something is still wrong and you don't see the alerts in the web GUI, then we need to pivot and try some other method. The next suggested step is a bit too much at this stage but will get you through the task. Click Here for the Event Level Troubleshooting or [here](https://mysticwayfarer7.github.io/mssp-soc/2020/04/04/alarms-notcoming-alienvault/) for OSSIM agent troubleshoot if alarms are not coming.

