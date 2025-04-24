## Script: Check SQL Server Services and Status (sys.dm_server_services)

**Description**:
This script returns information about all SQL Server–related services on the current instance, including their startup type, status, service account, cluster info, and process ID. It uses the DMV `sys.dm_server_services`.

**What It Shows**:
- Service name and executable path
- Whether it's running or stopped
- Last time the service was started
- Startup type (auto/manual/disabled)
- Whether it's part of a failover cluster
- Service account used to run it
- OS process ID

**Use Case**:
- Confirm SQL Server services are running
- Check if Agent or Browser service is stopped
- Troubleshoot service account or failover setup
- Audit startup type and service availability

**Requirements**:
- SQL Server 2008 R2 or later
- `VIEW SERVER STATE` permission
