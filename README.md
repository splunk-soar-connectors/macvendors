# MAC Vendors

Publisher: Splunk <br>
Connector Version: 2.1.11 <br>
Product Vendor: MAC Vendors <br>
Product Name: MAC Vendors <br>
Minimum Product Version: 5.1.0

Integrates with the MAC Vendors service to implement investigative actions

### Supported Actions

[test connectivity](#action-test-connectivity) - Validate the asset configuration for connectivity <br>
[lookup mac](#action-lookup-mac) - Query the Mac Vendor based on the OUI

## action: 'test connectivity'

Validate the asset configuration for connectivity

Type: **test** <br>
Read only: **True**

#### Action Parameters

No parameters are required for this action

#### Action Output

No Output

## action: 'lookup mac'

Query the Mac Vendor based on the OUI

Type: **investigate** <br>
Read only: **True**

#### Action Parameters

PARAMETER | REQUIRED | DESCRIPTION | TYPE | CONTAINS
--------- | -------- | ----------- | ---- | --------
**mac** | required | MAC address to lookup | string | `mac address` |

#### Action Output

DATA PATH | TYPE | CONTAINS | EXAMPLE VALUES
--------- | ---- | -------- | --------------
action_result.parameter.mac | string | `mac address` | d0:a6:37:aa:bb:cc |
action_result.data.\*.vendor | string | | Apple, Inc. |
action_result.status | string | | success failed |
action_result.message | string | | Vendor found: True |
action_result.summary.vendor_found | boolean | | True False |
summary.total_objects | numeric | | 1 |
summary.total_objects_successful | numeric | | 1 |

______________________________________________________________________

Auto-generated Splunk SOAR Connector documentation.

Copyright 2025 Splunk Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and limitations under the License.
