## Cloud Provider:
  * Amazon
## Instances:
  * 34.248.85.125 - ec2-34-248-85-125.eu-west-1.compute.amazonaws.com
  * 34.249.143.14 - ec2-34-249-143-145.eu-west-1.compute.amazonaws.com
  * 34.252.98.137 - ec2-34-252-98-137.eu-west-1.compute.amazonaws.com
  * 52.215.86.7 - ec2-52-215-86-7.eu-west-1.compute.amazonaws.com
  * 52.215.87.122 - ec2-52-215-87-122.eu-west-1.compute.amazonaws.com
## Linux Release:  
* [ec2-user@ip-172-31-17-209 ~]$ cat /proc/version

* Linux version 3.10.0-229.el7.x86_64 (mockbuild@x86-035.build.eng.bos.redhat.com) (gcc version 4.8.3 20140911 (Red Hat 4.8.3-7) (GCC) ) #1  SMP Thu Jan 29 18:37:38 EST 2015

## File System Capacity:  

* [ec2-user@ip-172-31-17-209 ~]$ df -h

    * Filesystem      Size  Used Avail Use% Mounted on
    * /dev/xvda2      120G  1.5G  119G   2% /

## Yum repolist enabled:  
[root@ip-172-31-17-209 ~]# yum repolist enabled
* Loaded plugins: amazon-id, rhui-lb
* repo id                                                            repo name                                                                         status
* !rhui-REGION-client-config-server-7/x86_64                         Red Hat Update Infrastructure 2.0 Client Configuration Server 7                        6
* !rhui-REGION-rhel-server-releases/7Server/x86_64                   Red Hat Enterprise Linux Server 7 (RPMs)                                          14,282
* !rhui-REGION-rhel-server-rh-common/7Server/x86_64                  Red Hat Enterprise Linux Server 7 RH Common (RPMs)                                   228
* repolist: 14,516

## List /etc/passwd: 

* [root@ip-172-31-17-209 ~]# egrep 'zhou|chen' /etc/passwd
 *  zhou:x:2800:2800::/home/zhou:/bin/bash
 * chen:x:2900:2900::/home/chen:/bin/bash

## List /etc/group: 

* [root@ip-172-31-17-209 ~]# egrep 'shanghai|beijing' /etc/group
 * shanghai:x:2901:chen
 * beijing:x:2902:zhou
