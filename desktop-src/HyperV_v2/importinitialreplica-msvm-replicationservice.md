---
Description: Imports the initial replication for a virtual machine.
ms.assetid: 151211fe-e58e-4fd4-87cd-cdb2ad55c0b1
title: ImportInitialReplica method of the Msvm_ReplicationService class
ms.topic: article
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- Msvm_ReplicationService.ImportInitialReplica
api_type: 
- COM
api_location: 
- vmms.exe
---

# ImportInitialReplica method of the Msvm\_ReplicationService class

Imports the initial replication for a virtual machine.

## Syntax


```mof
uint32 ImportInitialReplica(
  [in]  CIM_ComputerSystem REF ComputerSystem,
  [in]  string                 InitialReplicationImportLocation,
  [out] CIM_ConcreteJob    REF Job
);
```



## Parameters

<dl> <dt>

*ComputerSystem* \[in\]
</dt> <dd>

A reference to a [**CIM\_ComputerSystem**](https://docs.microsoft.com/windows/desktop/CIMWin32Prov/cim-computersystem) instance that represents the virtual machine for which the initial replication should be imported.

</dd> <dt>

*InitialReplicationImportLocation* \[in\]
</dt> <dd>

The fully qualified path of the directory from which the initial replication is to be imported. This cannot be **Null**.

</dd> <dt>

*Job* \[out\]
</dt> <dd>

If the operation is performed asynchronously, this method will return 4096, and this parameter will contain a reference to an object derived from [**CIM\_ConcreteJob**](https://docs.microsoft.com/previous-versions//cc136808(v=vs.85)).

</dd> </dl>

## Return value

This method returns one of the following values.

<dl> <dt>

**Completed with No Error** (0)
</dt> <dt>

**Method Parameters Checked - Job Started** (4096)
</dt> <dt>

**Failed** (32768)
</dt> <dt>

**Access Denied** (32769)
</dt> <dt>

**Not Supported** (32770)
</dt> <dt>

**Status is unknown** (32771)
</dt> <dt>

**Timeout** (32772)
</dt> <dt>

**Invalid parameter** (32773)
</dt> <dt>

**System is in use** (32774)
</dt> <dt>

**Invalid state for this operation** (32775)
</dt> <dt>

**Incorrect data type** (32776)
</dt> <dt>

**System is not available** (32777)
</dt> <dt>

**Out of memory** (32778)
</dt> <dt>

**File not found** (32779)
</dt> </dl>

## Requirements



|                                     |                                                                                                         |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 8 \[desktop apps only\]<br/>                                                              |
| Minimum supported server<br/> | Windows Server 2012 \[desktop apps only\]<br/>                                                    |
| Namespace<br/>                | Root\\Virtualization\\V2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>WindowsVirtualization.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## See also

<dl> <dt>

[**Msvm\_ReplicationService**](msvm-replicationservice.md)
</dt> </dl>

 

 




