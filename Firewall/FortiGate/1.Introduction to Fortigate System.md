# Introduction to Fortigate System

## 1. System Configuration Guide

To configure hostname first we need to enter into system global config mode by using *"config system global"* then follow the commmands to set hostname for the firewall as shown below.

```python
FortiGate-VM64-KVM # config system global
FortiGate-VM64-KVM (global) # set hostname LocalLabFw01
FortiGate-VM64-KVM (global) # end
LocalLabFw01 #
```


## 2. System & Interface Level Troubleshoot Guide 

### 2.1 General system information

To view general system information like last reboot reason, system uptime, Hostname, Fortigate Firewall version etc.,

```python
LocalLabFw01 # get system status
```

### 2.2 Interface [Port] Troubleshoot
 
 #### 2.2.1 Verify Interface Configuration

 To verify the interface configuration use **show system interface**  in cli this gives the listed interface along with it's configuration as shown in the fig 1.1

To view all the interface configuration we can execute below mentioned command.

```python
LocalLabFw01 # show system interface
```

We can use below mentioned command to view Specific port configuration

>Note: For example I've taken the First port of the Firewall. we can also check  configuration or status of any ports in the firewall 

```python
LocalLabFw01 # show system interface port1
```

#### 2.2.2 To view Full-configuration of the interface

```python
LocalLabFw01 # show full-configuration system interface port1
```

#### 2.2.3 To view the Interface status

This prints all the interface status in a single output.

```python
LocalLabFw01 # get system interface physical
```
To check specific Interface status.

```python
LocalLabFw01 # get system interface physical port1
```


