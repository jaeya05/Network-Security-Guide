# IPSEC Troubleshooting

## 1. Troubleshooting commands in Fortigate Firewall

* Enable timestamp and extend debug duration

```python
 lab-mplsFw01 # diagnose debug console timestamp enable


```

* Depending on how long debugging should continue, we can set a debug output limit. 

```python
lab-mplsFw01 # diagnose debug duration <N>
<Integer>   Duration in minutes, min = 1, max = 99999, 0 means unlimited.

lab-mplsFw01 # >
```

>Note: "0" to unlimited (diabling the feature), default 30minutes

* Filter remote peer public IP before running any debug when there is multiple tunnels

```python
lab-mplsFw01 # diagnose vpn ike log-filter dst-addr4 <peer ip>
```

>Note: Support multiple remote IP's while troubleshooting ADVPN
```python
lab-mplsFw01 # diagnose vpn ike log-filter mdst-addr4 <peer ip-1> <peer ip-2>
```

* Filter based on VDOM

```python
lab-mplsFw01 # diagnose vpn ike log-filter vd <vdom index>
```
* IKE debug commands

Enable all IKE debug level

```python
lab-mplsFw01 # diagnose debug application ike -1
Debug messages will be on for 30 minutes.

lab-mplsFw01 #

```
IKE debug without payload

```python
lab-mplsFw01 # diagnose debug application ike 127
```

Diable IKE debug

```python

lab-mplsFw01 # diagnose debug application ike 0

lab-mplsFw01 #
```
