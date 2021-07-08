---
layout: post
title: Alien Vault - Backups
---


### Alarm Backup – AlienVault 

* Login via WinSCP to the Server.

* Go to this path:

    /var/alienvault/backup/

* File name should be like: Configuration_CLIENT-AIO_1429616586.tar.gz

* Copy Alarm file to the local machine in any folder (E.g: C:\Backup)


STEPS


### Raw Log Backup – AlienVault

* Login via WinSCP to the Server.

* Be at this path:
  /var/ossim/logs/Year/Month/Day
  
* Copy the folder (Day) to the local machine in the folder Copy Alarm file to the local machine in any folder (E.g: C:\Backup)


### Event Backup– AlienVault 

* Login via WinSCP to the Server.

* Be at this path:

/var/lib/ossim/backup

* Copy the folder (Day) to the local machine in any folder (E.g: C:\Backup)
