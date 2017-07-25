# VSFTPd Add-on for Splunk

This CIM compliant TA can be used with Splunk (Enterprise Security) and provides
field extractions, aliases, eventtypes and tags for vsftpd logging.

It extracts fields and maps to the following Splunk CIM datamodels:

- Authentication
- Change analysis, for creation, reading, changng and deletion

## Installation

Install this TA on your Splunk (Enterprise Security) search head. Make sure to
name it TA-vsftpd otherwise ES won't eat it. 

## Configuration

Deploy an inputs.conf file like this on the FTP server:

```
[monitor:///var/log/vsftpd.log]
index = ftp
sourcetype = vsftpd
disabled = 0
```

## Support

This is an MIT licensed open source project without warranty of any kind. No
support is provided. A public repository and issue tracker are available at
[https://github.com/jorritfolmer/TA-vsftpd](https://github.com/jorritfolmer/TA-vsftpd)
