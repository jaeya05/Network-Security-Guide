# T shoot Guide

## 1.1 Verify General systemt information

To view general information of the system, which display informations like last reboot reason, system uptime, Hostname, Fortigate version etc.,

```bash
FG01-LocalLab # get system status
```

>OUTPUT

```bash
Version: FortiGate-VM64-KVM v7.2.4,build1396,230131 (GA.F)
Virus-DB: 1.00000(2018-04-09 18:07)
Extended DB: 1.00000(2018-04-09 18:07)
Extreme DB: 1.00000(2018-04-09 18:07)
AV AI/ML Model: 0.00000(2001-01-01 00:00)
IPS-DB: 6.00741(2015-12-01 02:30)
IPS-ETDB: 6.00741(2015-12-01 02:30)
APP-DB: 6.00741(2015-12-01 02:30)
INDUSTRIAL-DB: 6.00741(2015-12-01 02:30)
IPS Malicious URL Database: 1.00001(2015-01-01 01:01)
IoT-Detect: 0.00000(2022-08-17 17:31)
Serial-Number: FGVM00000000000000
License Status: Invalid Copy
VM Resources: 1 CPU/1 allowed, 1993 MB RAM
Log hard disk: Available
Hostname: FG01-LocalLab
Private Encryption: Disable
Operation Mode: NAT
Current virtual domain: root
Max number of virtual domains: 10
Virtual domains status: 1 in NAT mode, 0 in TP mode
Virtual domain configuration: disable
FIPS-CC mode: disable
Current HA mode: standalone
Branch point: 1396
Release Version Information: GA
FortiOS x86-64: Yes
System time: Thu May  4 12:15:48 2023
Last reboot reason: warm reboot
FG01-LocalLab #
```


# 2.Interface [Port] Troubleshoot
 
 ## 2.1 Verify Interface status

 To verify the interface configuration input **show system interface**  in cli will display the listed interface along with it's configuration as shown in the fig 1.1

```bash
Jaeya05-labFw-01 # show system interface
```
### 
