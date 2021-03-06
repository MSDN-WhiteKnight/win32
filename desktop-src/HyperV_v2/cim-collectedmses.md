---
Description: Represents a generic association between a collection of managed system elements and the members of the collection.
ms.assetid: c9e2bbca-67be-41f2-a94c-cf4eaf5f4694
title: CIM_CollectedMSEs class
ms.topic: article
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- CIM_CollectedMSEs
- CIM_CollectedMSEs.Collection
- CIM_CollectedMSEs.Member
api_type: 
- DllExport
api_location: 
- vmms.exe
---

# CIM\_CollectedMSEs class

Represents a generic association between a collection of managed system elements and the members of the collection.

## Syntax

``` syntax
[Association, Aggregation, Abstract, Version("2.6.0"), UMLPackagePath("CIM::Core::Collection"), AMENDMENT]
class CIM_CollectedMSEs : CIM_MemberOfCollection
{
  CIM_CollectionOfMSEs     REF Collection;
  CIM_ManagedSystemElement REF Member;
};
```

## Members

The **CIM\_CollectedMSEs** class has these types of members:

-   [Properties](#properties)

### Properties

The **CIM\_CollectedMSEs** class has these properties.

<dl> <dt>

**Collection**
</dt> <dd> <dl> <dt>

Data type: **CIM\_CollectionOfMSEs**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Aggregate**](https://docs.microsoft.com/windows/desktop/WmiSdk/standard-qualifiers), [**Override**](https://docs.microsoft.com/windows/desktop/WmiSdk/standard-qualifiers) ("Collection")
</dt> </dl>

The collection.

</dd> <dt>

**Member**
</dt> <dd> <dl> <dt>

Data type: **CIM\_ManagedSystemElement**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://docs.microsoft.com/windows/desktop/WmiSdk/standard-qualifiers) ("Member")
</dt> </dl>

The members of the collection.

</dd> </dl>

## Requirements



|                                     |                                                                                                         |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 10 \[desktop apps only\]<br/>                                                             |
| Minimum supported server<br/> | Windows Server 2016<br/>                                                                          |
| Namespace<br/>                | Root\\virtualization\\v2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>WindowsVirtualization.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## See also

<dl> <dt>

[**CIM\_MemberOfCollection**](cim-memberofcollection.md)
</dt> </dl>

 

 




