---
Description: Turns off subclassing for the specified control.
ms.assetid: d4d34624-7d85-4c53-8318-b3e5d6f95f7a
title: Ctl3dUnsubclassCtl function
ms.topic: article
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- Ctl3dUnsubclassCtl
api_type: 
- DllExport
api_location: 
- Ctl3d32.dll
---

# Ctl3dUnsubclassCtl function

Turns off subclassing for the specified control.

## Syntax


```C++
BOOL WINAPI Ctl3dUnsubclassCtl(
   HWND hwnd
);
```



## Parameters

<dl> <dt>

*hwnd* 
</dt> <dd>

A handle to the control window.

</dd> </dl>

## Return value

Returns **TRUE** if the control is successfully subclassed; otherwise, it returns **FALSE**.

## Remarks

This function has no associated import library or header file; you must call it using the [**LoadLibrary**](https://msdn.microsoft.com/en-us/library/ms684175(v=VS.85).aspx) and [**GetProcAddress**](https://msdn.microsoft.com/en-us/library/ms683212(v=VS.85).aspx) functions.

## Requirements



|                |                                                                                        |
|----------------|----------------------------------------------------------------------------------------|
| DLL<br/> | <dl> <dt>Ctl3d32.dll</dt> </dl> |



## See also

<dl> <dt>

[**Ctl3dSubclassCtl**](ctl3dsubclassctl.md)
</dt> </dl>

 

 




