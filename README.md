[comment]: # "Auto-generated SOAR connector documentation"
# MAC Vendors

Publisher: Splunk  
Connector Version: 2\.1\.8  
Product Vendor: MAC Vendors  
Product Name: MAC Vendors  
Product Version Supported (regex): "\.\*"  
Minimum Product Version: 5\.1\.0  

Integrates with the MAC Vendors service to implement investigative actions

### Supported Actions  
[test connectivity](#action-test-connectivity) - Validate the asset configuration for connectivity  
[lookup mac](#action-lookup-mac) - Query the Mac Vendor based on the OUI  

## action: 'test connectivity'
Validate the asset configuration for connectivity

Type: **test**  
Read only: **True**

#### Action Parameters
No parameters are required for this action

#### Action Output
No Output  

## action: 'lookup mac'
Query the Mac Vendor based on the OUI

Type: **investigate**  
Read only: **True**

#### Action Parameters
PARAMETER | REQUIRED | DESCRIPTION | TYPE | CONTAINS
--------- | -------- | ----------- | ---- | --------
**mac** |  required  | MAC address to lookup | string |  `mac address` 

#### Action Output
DATA PATH | TYPE | CONTAINS
--------- | ---- | --------
action\_result\.parameter\.mac | string |  `mac address` 
action\_result\.data\.\*\.vendor | string | 
action\_result\.status | string | 
action\_result\.message | string | 
action\_result\.summary\.vendor\_found | boolean | 
summary\.total\_objects | numeric | 
summary\.total\_objects\_successful | numeric | 