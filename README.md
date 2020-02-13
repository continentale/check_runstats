# check_runstats

check_runstats is a nagios / icinga compliant check which validates running linux processes via SNMP.

## system requirements
PHP with mod_snmp installed.
```bash
sudo apt-get install php-snmp
sudo phpenmod snmp
```
## Usage Examples
##### SNMPV1
``` ./check_runstats -h=10.10.0.1 -C=public -v1 -k=processname```

##### SNMP V2
``` ./check_runstats -h=10.10.0.1 -C=public -k=processname```

##### SNMP V3
``` ./check_runstats -h=10.10.0.1 -u=snmpusername -p=password -e=SHA -E=AES -k=processname```
