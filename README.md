# Cisco-Packet-Tracer

## VLAN Setup on Switch

To add a device (connected with FastEthernet Port 0/1) to VLAN 101, simply write :

```
enable
configure terminal

interface fastEthernet 0/1

switchport mode access
switchport access vlan 101

no shutdown
exit

```

To add another device (connected with FastEthernet Port 0/4) to VLAN 101, simply write :

```
interface fastEthernet 0/4

switchport mode access
switchport access vlan 101

no shutdown
exit

```
To Trunk Switch port(Trunk switchs for accessing each other) instead of access just write trunk :

```
switchport mode trunk
```
After separting devices to different VLANs, save data permanently to non-volatile memory with this command:
```
do write memory
```

## Configuring Gigabit Ethernet LAN Interfaces

```
enable
configure terminal

interface gigabitethernet 0/0
ip address 192.168.0.10 255.255.255.0

no shutdown
exit

do write memory
```
