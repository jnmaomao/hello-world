# List the cloud provider you are using (AWS, GCE, Azure, other)
AWS-us-west-2c

# List the nodes you are using by IP address and name
public ip      private ip    hostname    
54.202.94.166  172.31.6.115 master.com ec2-54-202-94-166.us-west-2.compute.amazonaws.com
54.190.25.88 172.31.7.130  cmnode.com  ec2-54-190-25-88.us-west-2.compute.amazonaws.com 
54.245.142.180 172.31.11.141 datanode1.com ec2-54-245-142-180.us-west-2.compute.amazonaws.com
54.202.51.201 172.31.3.128 datanode2.com ec2-54-202-51-201.us-west-2.compute.amazonaws.com
54.202.54.174 172.31.13.250 datanode3.com ec2-54-202-54-174.us-west-2.compute.amazonaws.com

# List the Linux release you are using
CentOS6.5

# Demonstrate the disk capacity available on each node is >= 30 GB
/dev/xvde       7.9G  651M  6.9G   9% /
tmpfs           7.4G     0  7.4G   0% /dev/shm

# List the command and output for yum repolist enabled
[root@cmnode ~]# yum repolist enabled
Loaded plugins: fastestmirror, presto
base                                                                                                                                             | 3.7 kB     00:00     
base/primary_db                                                                                                                                  | 4.7 MB     00:00     
extras                                                                                                                                           | 3.4 kB     00:00     
extras/primary_db                                                                                                                                |  37 kB     00:00     
updates                                                                                                                                          | 3.4 kB     00:00     
updates/primary_db                                                                                                                               | 803 kB     00:00     
repo id                                                                    repo name                                                                              status
base                                                                       CentOS-6 - Base                                                                        6,706
extras                                                                     CentOS-6 - Extras                                                                         64
updates                                                                    CentOS-6 - Updates                                                                       252
repolist: 7,022

# Add the following Linux accounts to all nodes
User neymar with a UID of 2010
User ronaldo with a UID of 2016
Create the group barca and add ronaldo to it
Create the group merengues and add neymar to it



# List the /etc/passwd entries for neymar and ronaldo
Not the entire file!
neymar:x:2010:501::/home/neymar:/bin/bash
ronaldo:x:2016:500::/home/ronaldo:/bin/bash

# List the /etc/group entries for barca and merengues
Not the entire file!
barca:x:500:ronaldo
merengues:x:501:neymar
