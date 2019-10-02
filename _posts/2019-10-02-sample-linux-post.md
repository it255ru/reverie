```bash
[root@node4 ~]# lsblk
NAME          MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
sda             8:0    0    8G  0 disk
├─sda1          8:1    0  512M  0 part /boot
└─sda2          8:2    0  7.5G  0 part
  ├─rhel-root 253:0    0 16.1G  0 lvm  /
  └─rhel-swap 253:1    0  956M  0 lvm  [SWAP]
sdb             8:16   0   17G  0 disk
sdc             8:32   0   10G  0 disk
└─sdc1          8:33   0   10G  0 part
  └─rhel-root 253:0    0 16.1G  0 lvm  /
sr0            11:0    1  6.5G  0 rom
sr1            11:1    1 1024M  0 rom

[root@node4 ~]# dnf install boom-boot -y
Updating Subscription Management repositories.
Last metadata expiration check: 12:44:30 ago on Thu 20 Jun 2019 12:00:09 AM IST.
Dependencies resolved.
==========================================================================================
 Package                          Arch             Version           Repository
==========================================================================================
Installing:
 boom-boot                        noarch           0.9-5.el8         rhel_dvd_baseos
Installing dependencies:
 boom-boot-conf                   noarch           0.9-5.el8         rhel_dvd_baseos
 python3-boom                     noarch           0.9-5.el8         rhel_dvd_baseos
Installing weak dependencies:
 boom-boot-grub2                  noarch           0.9-5.el8         rhel_dvd_baseos

Transaction Summary
==========================================================================================
Install  4 Packages

Total size: 443 k
Installed size: 2.2 M
Downloading Packages:
Running transaction check
Transaction check succeeded.
Running transaction test
Transaction test succeeded.
Running transaction
  Preparing        :
Installed: boom-boot-conf-0.9-5.el8.noarch
  Installing       : boom-boot-conf-0.9-5.el8.noarch
Installed: boom-boot-conf-0.9-5.el8.noarch
Installed: python3-boom-0.9-5.el8.noarch
  Installing       : python3-boom-0.9-5.el8.noarch
Installed: python3-boom-0.9-5.el8.noarch
Installed: boom-boot-grub2-0.9-5.el8.noarch
  Installing       : boom-boot-grub2-0.9-5.el8.noarch
Installed: boom-boot-grub2-0.9-5.el8.noarch
Installed: boom-boot-0.9-5.el8.noarch
  Installing       : boom-boot-0.9-5.el8.noarch
Installed: boom-boot-0.9-5.el8.noarch
  Running scriptlet: boom-boot-0.9-5.el8.noarch
  Verifying        : boom-boot-0.9-5.el8.noarch
  Verifying        : boom-boot-conf-0.9-5.el8.noarch
  Verifying        : boom-boot-grub2-0.9-5.el8.noarch
  Verifying        : python3-boom-0.9-5.el8.noarch

Installed:
  boom-boot-0.9-5.el8.noarch    boom-boot-grub2-0.9-5.el8.noarch      boom-boot-conf-0.9-5.el8.noarch   python3-b

Complete!
```
