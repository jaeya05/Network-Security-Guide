# T shoot Guide

## 1.1 Verify General systemt information

To view general information of the system, which display informations like last reboot reason, system uptime, Hostname, Fortigate version etc.,

```bash
FG01-LocalLab # get system status
```

# 2.Interface [Port] Troubleshoot
 
 ## 2.1 Verify Interface status

 To verify the interface configuration input **show system interface**  in cli will display the listed interface along with it's configuration as shown in the fig 1.1

```bash
Jaeya05-labFw-01 # show system interface
```
### 2.1.1 To view Full-configuration of the interface

```bash
FG01-LocalLab # show full-configuration system interface port1
```

>Note: For example I've taken the First port of the Firewall. we can check full configuration of any ports in the firewall 
