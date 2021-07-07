---
layout: post
title: Alien Vault Alarms Not Recevied
---



For all MSSPs or users who are working with Alien Vault as a SIEM solution in their enterpise infrastructure it is common to get into problem because of alarms not being triggered in the SIEM solution. Now this could happen for multiple reasons which requires troubleshooting across the whole data piple line and finding the point where things are broked or need a little push.

Some of the options that can be pursued to troubleshoot and resolve this issue have been mentioned below:


* Login to Alien Vault server using putty with “root” credentials.
* After login, you will see the following screen.

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/4.png "Alien Vault Console Login Page")

* Select the “Jailbreak System”
* Click “Yes” or Press “Enter” from the keyboard and accept the “Jailbreak Commandline Notice” in next screen by clicking “Yes:”

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/5.png "Alien Vault Confirmation")

* This will give you a command line access to Alien Vault server and screen will be displayed as below.

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/5.png "Alien Vault Confirmation")

* Run the following command in the console and wait for this to complete. Command: /etc/init.d/ossim-agent restart

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/6.png "OSSIM Agent Restart")

* If the above command ran successfully, wait for at least 5 minutes and refresh the Alien Vault Alarms page in browser.

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/7.png "Alien Vault Browser GUI")

If something is still wrong and you don't see the alerts in the web GUI, then we need to pivot and try some other method. The next suggested step is a bit too much at this stage but will get you through the task. Click Here for the Alien Vault Reconfiguration

