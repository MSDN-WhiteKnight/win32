---
Description: The get\_SourceLeft method retrieves the left coordinate of the current source rectangle.
ms.assetid: dbfb1850-6e49-481c-b26a-22ccb9e4455a
title: CBaseControlVideo.get_SourceLeft method
ms.topic: article
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- CBaseControlVideo.get_SourceLeft
api_type: 
- COM
api_location: 
- Strmbase.lib
- Strmbase.dll
- Strmbasd.lib
- Strmbasd.dll
---

# CBaseControlVideo.get\_SourceLeft method

The `get_SourceLeft` method retrieves the left coordinate of the current source rectangle.

## Syntax


```C++
HRESULT get_SourceLeft(
   long *pSourceLeft
);
```



## Parameters

<dl> <dt>

*pSourceLeft* 
</dt> <dd>

Pointer to the left coordinate of the current source rectangle.

</dd> </dl>

## Return value

Returns an **HRESULT** value that depends on the implementation; can be one of the following values, or other values not listed.



| Return code                                                                                           | Description                                                                      |
|-------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| <dl> <dt>**E\_FAIL**</dt> </dl>                | Failure.<br/>                                                              |
| <dl> <dt>**E\_POINTER**</dt> </dl>             | **NULL** pointer argument.<br/>                                            |
| <dl> <dt>**VFW\_E\_NOT\_CONNECTED**</dt> </dl> | The operation cannot be performed because the pins are not connected.<br/> |
| <dl> <dt>**NOERROR**</dt> </dl>                | Success.<br/>                                                              |



 

## Remarks

An application can change the source and destination rectangles for the video through the [**IBasicVideo**](/windows/desktop/api/Control/nn-control-ibasicvideo) interface. The source rectangle affects which section of the native video source will appear on the display; the destination rectangle affects where the video will appear when played. The destination rectangle is relative to the client area of the window in which it is playing. The upper-left corner of the window is coordinate (0,0).

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Ctlutil.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CBaseControlVideo Class**](cbasecontrolvideo.md)
</dt> </dl>

 

 




