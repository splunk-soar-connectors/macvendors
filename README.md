[comment]: # "Auto-generated SOAR connector documentation"
# MAC Vendors

Publisher: Splunk  
Connector Version: 2.1.9  
Product Vendor: MAC Vendors  
Product Name: MAC Vendors  
Product Version Supported (regex): ".\*"  
Minimum Product Version: 5.1.0  

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
DATA PATH | TYPE | CONTAINS | EXAMPLE VALUES
--------- | ---- | -------- | --------------
action_result.parameter.mac | string |  `mac address`  |   d0:a6:37:aa:bb:cc 
action_result.data.\*.vendor | string |  |   Apple, Inc. 
action_result.status | string |  |   success  failed 
action_result.message | string |  |   Vendor found: True 
action_result.summary.vendor_found | boolean |  |   True  False 
summary.total_objects | numeric |  |   1 
summary.total_objects_successful | numeric |  |   1 