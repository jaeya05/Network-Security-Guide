# Introduction to Fortigate System

## 1. System Configuration Guide

To configure hostname first we need to enter into system global config mode by using *"config system global"* then follow the commmands to set hostname for the firewall as shown below.

```bash
FortiGate-VM64-KVM # config system global
FortiGate-VM64-KVM (global) # set hostname FG01-LocalLab
FortiGate-VM64-KVM (global) # end
FG01-LocalLab #
```


## 2. System & Interface Level Troubleshoot Guide 

### 2.1 General system information

To view general system information like last reboot reason, system uptime, Hostname, Fortigate Firewall version etc.,

```bash
FG01-LocalLab # get system status
```

### 2.2 Interface [Port] Troubleshoot
 
 #### 2.2.1 Verify Interface Configuration

 To verify the interface configuration use **show system interface**  in cli this gives the listed interface along with it's configuration as shown in the fig 1.1

To view all the interface configuration we can execute below mentioned command.

```bash
FG01-LocalLab # show system interface
```

We can use below mentioned command to view Specific port configuration

>Note: For example I've taken the First port of the Firewall. we can also check  configuration or status of any ports in the firewall 

```bash
FG01-LocalLab # show system interface port1
```

#### 2.2.2 To view Full-configuration of the interface

```bash
FG01-LocalLab # show full-configuration system interface port1
```

#### 2.2.3 To view the Interface status

This prints all the interface status in a single output.

```bash
FG01-LocalLab # get system interface physical
```
To check specific Interface status.

```bash
FG01-LocalLab # get system interface physical port1
```