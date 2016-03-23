# TA-vsftpd for Splunk

This CIM compliant TA can be used with Splunk (Enterprise Security) and provides
field extractions, aliases, eventtypes and tags for vsftpd logging.

It extracts fields and maps to the following Splunk CIM datamodels:

- Authentication
- Change analysis, for creation, reading, changng and deletion

## Installation

Install this TA on your Splunk (Enterprise Security) search head. Make sure to
name it TA-vsftpd otherwise ES won't eat it. 

## Configuration

This TA expects vsftpd logging to be sourcetyped `vsftpd`.  If you use a
different sourcetype, you should change `props.conf` accordingly in
this TA.

