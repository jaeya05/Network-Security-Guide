# T-shoot Guide

## 1.General systemt information

To view general system information like last reboot reason, system uptime, Hostname, Fortigate Firewall version etc.,

```bash
FG01-LocalLab # get system status
```

## 2.Interface [Port] Troubleshoot
 
 ## 2.1 Verify Interface Configuration

 To verify the interface configuration use **show system interface**  in cli this gives the listed interface along with it's configuration as shown in the fig 1.1

To view all the interface configuration we can execute below mentioned command.

```bash
FG01-LocalLab # show system interface
```

We can use below mentioned command to view Specific port configuration

>Note: For example I've taken the First port of the Firewall. we can check  configuration or status of any ports in the firewall 

```bash
FG01-LocalLab # show system interface port1
```

### 2.1.1 To view Full-configuration of the interface

```bash
FG01-LocalLab # show full-configuration system interface port1
```

### 2.1.2 To view the Interface status

This prints all the interface status in a single output.

```bash
FG01-LocalLab # get system interface physical
```
To check specific Interface status we can use the below one.

```bash
FG01-LocalLab # get system interface physical port1
```