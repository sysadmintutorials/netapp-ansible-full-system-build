# NetApp Ansible Playbooks

#### Date: 3-8-2019
#### Version: 1
#### Blog: www.sysadmintutorials.com
#### Twitter: @systutorials

## Description

Contained within this repository are NetApp Ansible playbooks

## File Listing & Description
1. 00_netapp_full_install.yml<br>
   
   This playbook is part of my blog post - www.sysadmintutorials.com/how-to-automate-netapp-installations-with-ansible<br>
   
   It will setup a NetApp cluster ready for VMware vSphere NFS datastores. It performs the following:
```sh
    - Set NTP
    - Set Timezone
    - Rename the Root Aggregate
    - Create and online a new Data Aggregate
    - Create a Vserver
    - Setup a VLAN
    - Creating a Broadcast Domain
    - Subnet Creation
    - Creating an NFS Lif
    - Start NFS
    - Create NFS Export Rule
    - Add DNS Settings to Vserver
    - Create first NFS Volume
    - Create an additional NFS Volume
 ```
 
 Be sure to change the variables within the yml file to match your environment
 
 To run this ansible playbook simply execute: ansible-playbook 00_netapp_full_install.yml
