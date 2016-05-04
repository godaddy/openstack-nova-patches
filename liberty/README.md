# Liberty Patches

These patches are cumulative, so in most cases you must have applied all
previous patches in order for them to apply cleanly.

### 0002-enable-Aggreagete-API-in-cells.patch

Enable Aggregate API in cells * Source: Nectar * Orig patch: 0002-enable-Aggreagete-API-in-cells.patch * Verified: Ran all imported/modified unit test cases ran all success

### 0003-use-sysmetadata-to-get-instance-az-in-api-cell.patch

Use Sysmetadata to get instance AZ in API Cell * Source: Nectar * Orig patch: 0003-use-sysmetadata-to-get-instance-az-in-api-cell.patch * Removed unused ref: from nova import db

### 0004-enable-AZ-with-cells.patch

Enable Availability Zones with Cells * Source: Nectar * Orig patch: 0004-enable-AZ-with-cells.patch

### 0005-enable-flavor-create-with-cells.patch

Enable flavor creation with Cells * Source: Nectar * Orig patch: 0005-enable-flavor-create-with-cells.patch

### 0006-Filter-cell-capacity-report-by-aggregate-metadata.patch

Filter cell capacity report by aggregate metadata * Source: Nectar * Orig patch: 0006-Filter-cell-capacity-report-by-aggregate-metadata.patch

### 0007-Print-cell-name-in-timeout-exceptions.patch

Print cell name in timeout exceptions.patch * Source: Nectar * Orig patch: 0007-Print-cell-name-in-timeout-exceptions.patch

### 0008-expire-reservation-in-cells-manager.patch

Expire reservation in cells manager * Source: Nectar * Orig patch: 0008-expire-reservation-in-cells-manager.patch * Removed obsolete obsolete and redundant periodic_task import * Re-ran test_cells_manager.py tests with all passing.

### 0009-api-server-read-cell-state-from-db.patch

API server read cell state from DB * Source: Nectar * Orig patch: 0009-api-server-read-cell-state-from-db.patch * Re-ran test_db_api.py tests with all passing.

### 0010-use-sysmetadata-to-get-instance_name-in-api-cell.patch

Use sysmetadata to get instance_name in api cell * Source: Nectar * Orig patch: 0010-use-sysmetadata-to-get-instance_name-in-api-cell.patch

### 0011-send-up-AZ-and-instance_name-in-sysmetdata.patch

Send up AZ and instance_name in sysmetdata * Source: Nectar * Orig patch: 0011-send-up-AZ-and-instance_name-in-sysmetdata.patch * Upstream removed param "update_cells=True" from update_instance calls. * * Added param back in. * * Not 100% sure all previous uses of this were ever called with False. * Tests test_compute and test_db_api both ran without issues.

### 0012-review-184155-support-attach-detach-interface-and-external-events.patch

Review 184155 Support attach detach interface and external events * Source: OpenStack : https://review.openstack.org/#/c/184155 * Orig patch: 0012-review-184155-support-attach-detach-interface-and-external-events.patch * Changed rpc version from 1.36 to 1.34.1. This affected rpcapi and test_cells_rpcapi. * Tests test_cells_manager, test_cells_messaging, and test_cells_rpcapi ran without issues.

### 0014-kilo-cells-spice-console-fix.patch

Kilo cells spice console fix * Source: GoDaddy * Orig patch: 0014-kilo-cells-spice-console-fix.patch * Modified slightly to not define metas var and pass in expected_attrs directly * Tests test_compute (has refs to get_spice_console) without issues.

### 0015-port-instance-info-cache-with-cells.patch

Port instance info cache with cells * Source: Nectar * Orig patch: 0015-port-instance-info-cache-with-cells.patch * Upstream moved method get_instance_nw_info from network/neutronv2/api.py to network/base_api.py * Refactored original patch to apply the diffs for that method into base_api.py with update_cells as param. Tests showed it was called with various values of True/False. * Unit tests test_compute_api and test_neutronv2(and others) ran successfully without issues.

### 0018-server-groups-cells-support.patch

Server groups cells support * Source: GD * Orig patch: 0018-server-groups-cells-support.patch * Upstream moved method server_groups to legacy_v2/contribs * Refactored slightly to import webob exceptions into API * Unit tests run across several major testers with all passing.
