---
layout: post
title: Verifying Malicious IOCs on Virus Total
---

Virus Total is a website that provides free service to evaluate files adn scan them across different security vendor's products. We are able to upload files, add urls or IPs into the search bar and this will be searched across all security vendors and results are shown in the form of a report.This post and many to come are the activities which were done by me as a knowledge transfer sessions for my team while setting up an MSSP to provide SOC sesrvices to our various clients in Saudi Arabia.

### VERIFY IP / HASH / DOMAIN NAME

To check if the IP, hash or filename is malicious or not, simply copy the IP/hash and paste it on the textbox in Virus total.
Open the Google Chrome Browser or any other prefered web browser, in the address bar type https://www.virustotal.com/ or [click here](https://www.virustotal.com/).

Once the page loads, you should see something similar to this:

![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/1.png "Virus Total Main Page")

Note that there are three tabs,
* File: Use this option incase you have a malicious file and you'd like to see if it is malicious.
* URL: Select this Option if you have any URL that you have found in logs, or client has shared to see the reputation of the URL.
* Search: Select this tab, if you want to search for any IP, Hash or domain name to verify if this is malicious or a clean artifact.

### EXAMPLE

* Copy the malicious IP using CTRL + C (from keyboard) or by using the mouse select the text of IP and make a right click and select Copy.
* Go to Google chrome browser or your preffered browser, in the address bar, make one left-click and type the following URL. https://www.virustotal.com
* Once the page has been loaded, click on the search tab in the middle of the page and wait for the text box to appear.
* In the search tab, paste the malicious IP copied in step 1, you can paste using CTRL + V (from keyboard) or use mouse to make one right-click and click paste.
* The end result would be as following except the IP mentioned is a dummy ip being used as an example.


![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/2.png "Virus Total Search Page")

* Next click on the search icon (magnifier glass icon) at the right end of the textbox visible on the page.
* Wait for the page to load itself with results about the pasted IP.
* The result page would either report it as malicious or clean in the following way.


![alt text](https://mysticwayfarer7.github.io/mssp-soc/images/3.png "Virus Total Result Page")

* Even if one of the engine’s mentioned in the result report it as malicious, we will share with client the remedial steps.
* If all the engine’s mention ‘Clean’ next to their name as visible for some of the engines in above picture, it can be considered as safe.


