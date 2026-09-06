# CCNA-Self-made-Network-Lab
I have created this small lab to check that whether i can design network by myself or not.
<br>
Currently it has very basic design, few devices and basic configuration. I will work more on this lab and try to implement everything i learned in CCNA.
<br>
## Network Topology
<img width="1920" height="990" alt="Screenshot (21)" src="https://github.com/user-attachments/assets/bd99fa6c-4069-4c93-93b9-ad175e88f0dd" />

### Info-About Lab Network
In this network, ASW-1 has two Vlans configured on f0/1-2 and f0/3-4 named Vlan 10 for IT and Vlan 20 for Management respectively. Both links Between ASW-1 and DSW-1--DSW-2 are trunk links and native Vlan is un-used Vlan 1000. 
<br>
DSW-1 is HSRP active for Vlan 10 and standby for Vlan 20. DSW-2 is HSRP active for Vlan 20 and standby for Vlan 10 providing redundacy in the network.
<br>
R1 is configured as a DHCP server for both Vlans.
<br>
OSPF is configured to provide full connectivity in the network.
<br>
Etherchannel is configured between the two Distribution switches.
<br>

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
### This lab is still a work in progresss. I keep getting new ideas, and I am trying to bring them to life by implementing them in this network.   :)
