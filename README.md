# CCNA-Self-made-Network-Lab

## Network Topology
<img width="1920" height="1003" alt="Screenshot (23)" src="https://github.com/user-attachments/assets/03de519d-7d49-42da-a5ae-5d4fe1ac70fa" />

## Personal Note :)
This lab was mainly a personal test to see if i could design and build a working network from scratch using the concepts i have learned. it is simple and does'nt include every CCNA concept, but it represents my own ideas and approch to network design.


### Info-About Lab Network
In Office's network, ASW-1 has two Vlans configured on f0/1-2 and f0/3-4 named Vlan 10 for IT and Vlan 20 for Management respectively. Both links Between ASW-1 and DSW-1--DSW-2 are trunk links and native Vlan is un-used Vlan 1000.
<br>
In guest's network, there are 4 Access-layer switches. ASW1 and ASW2 both are connected to ASW-3/4 providing redundant links.
<br>
DSW-1 is HSRP active for Vlan 10 and standby for Vlan 20. DSW-2 is HSRP active for Vlan 20 and standby for Vlan 10 providing redundacy in the network.
<br>
In Guest's network R3 is active for guest's devices and R4 is standby.
<br>
R1 is configured as a DHCP server for both Vlans.
<br>
R2 is configured as a DHCP server for guests devices.
<br>
OSPF is configured to provide full connectivity in the network.
<br>
Etherchannel is configured between the two Distribution switches.
<br>
Server in Office network is configured as DNS-server for both, host devices in Office network and in Guests network

### Few Verification commands

show vlan brief
<br>
show standby brief
<br>
show interfaces trunk
<br>
show dhcp pool
<br>
show dhcp pool binding
<br>
show etherchannel summary
<br>
show ip ospf neighbor
<br>
show ip interfaces brief

