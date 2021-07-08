---
layout: post
title: Alien Vault Plugins Troubleshoot
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

* Depending on the plug in which you are troubleshooting, go to the defined log file for that plugin and run this command to see if the logs are being written on the log file. Please make sure that you have the correct log file for the plugin.

<div class="message">
  tail -f /path/to/<data-Source-name>.log
</div>

  For example, in our any client's deployment, if we have to check the log file for nxlog we will run the following command.

<div class="message">
  tail –f /var/log/nxlog.log
</div>

* If there is no logs being written in the above file, run the following command and then run the command in step 7 again.

<div class="message">
  /etc/init.d/rsyslog restart
</div>
  

 * If you see new messages in the log files, check the events in the browser 
  

