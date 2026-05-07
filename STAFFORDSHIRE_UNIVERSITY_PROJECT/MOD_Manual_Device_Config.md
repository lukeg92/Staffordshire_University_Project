**Manual device configurations**



**username:** Staffordshire

**password:** university

**privilege password:** staffordshire\_university



**switches only**



vlan 10

name STAFFORDSHIRE\_VLAN

no shut

vlan 20

name UNIVERSITY\_VLAN

no shut

vlan 30

name PROJECT\_VLAN

no shut



int eth0/1

switchport mode access

switchport access vlan 10

int eth0/2

switchport trunk encapsulation dot1q

switchport mode trunk

switchport trunk allowed vlan 10,20,30

int eth0/3

switchport trunk encapsulation dot1q

switchport mode trunk

switchport trunk allowed vlan 10,20,30



**Routers only**



**MOD-R1**

int eth0/1

ip address 192.168.1.1 255.255.255.0

no shut

int eth0/2

no shut

int eth0/3

no shut



**MOD-R2**

int eth0/1

ip address 192.168.1.2 255.255.255.0

no shut

int eth0/2

no shut

int eth0/3

no shut



**Both Routers OSPF**

router ospf 1

network 192.168.1.0 0.0.0.255 area 0



**All devices**



banner motd $

=================================================

Welcome to the MOD NetDevOps Project

All devices in this lab are configured by Ansible

All configurations are for demonstration purposes 

This does not reflect operational networks

=================================================

$



end 

copy run start



