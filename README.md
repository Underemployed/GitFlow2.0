
# Exp No: 2  
**Date:**  
## Familiarization of Internetworking Operating System and Configurations  

### Aim  
To study Internetworking Operating System (IOS) and its basic configurations.  

### Router Memory Components  
Cisco routers contain four types of memory: ROM, Flash, NVRAM, and RAM. ROM holds the bootstrap program (ROMmon), which runs POST on startup. Flash stores the IOS image, while NVRAM saves configurations.  

### User Vs Privileged Mode  
User mode is indicated with `>`, while privileged mode uses `ENABLE`.  
```
Router>  
Router>enable  
Router#
```  
### HELP  
Typing `?` displays available commands in the current mode. Using `show ?` lists all `show` commands.  
```
Router # show ?
```  

### Configuration Mode  
From privileged mode, enter configuration mode using `config t`. Exit using `exit` or `Ctrl+Z`.  
```
Router # config t  
Router(config )# exit or ^Z
```  

### Show Version  
`show version` provides details like router model, OS version, last boot time, memory, interfaces, and configuration register.  
```
Router# show version
```  

### Routing Protocols  
Use `show protocol` to view active routing protocols.  
```
Router>show protocol
```  

### Running Configuration  
The active configuration is called the running config. It is not saved automatically and must be stored manually using the `copy` command.  
```
Router# show running-config
```  

### Command History  
To view recent commands in memory, use:  
```
Router# show history
```  

### Clock  
The router maintains an internal clock. Check it using:  
```
Router# show clock
```  

### Host Tables  
You can create a list of hostnames and view them using:  
```
Router# show hosts
```  

### Show Interfaces  
This command provides statistics for all configured interfaces.  
```
Router# show interfaces
```  

### Hostname Configuration  
Set a router's hostname for identification:  
```
Router# config t  
Router(config)# hostname R1  
```  

### Examining Interfaces  
Routers have different interfaces like Ethernet, Serial, ISDN, etc. The `show interfaces` command provides details, while `show ip int brief` offers a summary.  
```
Router1# show ip int brief
```  

### Examining Controllers  
Controllers manage physical connections. The `show controller` command checks if the router is a DTE or DCE.  
```
Router# show controllers serial 0/0/1
```  

### Configuring Interfaces  
To activate a down interface, enter config mode and use `no shut`.  
```
Router# config  
Router(config)# int fastethernet 0/1  
Router(config-if)# no shut  
```  
For DCE interfaces, set a clock rate:  
```
Router(config)# interface serial 0/0/1  
Router(config-if)# clock rate 9600  
```  

### Show IP Route  
Displays routing table details.  
```
Router# show ip route
```  

### Basic IP Configuration and Verification  
Set an IP address for an interface using:  
```
Router(config)# int FastEthernet 0/1  
Router(config-if)# ip address 192.168.2.1 255.255.255.0  
Router(config-if)# no sh
```  

### Ping  
Tests connectivity by sending ICMP packets.  
```
Router# ping <IP address>
```  

### Backing Up and Restoring IOS  
TFTP transfers IOS images. Ensure connectivity before backup.  
```
Router# show flash:  
```  
To copy an IOS file to a TFTP server:  
```
Router# copy flash: tftp:
```  
To restore IOS in ROMmon mode:  
```
rommon 1> tftpdnld  
rommon 2 > IP_ADDRESS=192.168.1.1  
rommon 3 > TFTP_FILE=c2900-universalk9-mz.SPA.151-4.M4.bin  
```  
After copying, verify the file and reset the router.  

### Result  
Study of IOS, basic configurations, and backup & restoration has been completed.  
```
rommon 9 > reset
```  
