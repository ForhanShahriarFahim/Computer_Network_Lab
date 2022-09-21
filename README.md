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

## Router CLI command Format for assigning IP address:

```
enable
configure terminal

interface gigabitEthernet 0/1
ip address [gateway address] [subnet mask]
ip address 192.168.10.21 255.255.255.255
no shutdown
exit
do write memory
```
## Router CLI command Format for static routing

```
enable
configure terminal
ip route [destination network address] [subnet mask] [via ip]
ip route 192.168.50.0 255.255.255.0 192.168.90.91
```


