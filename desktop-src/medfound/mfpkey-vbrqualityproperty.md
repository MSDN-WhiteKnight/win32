---
Description: Specifies the actual quality level for quality based (1-pass) variable-bit-rate (VBR) encoding.
ms.assetid: e45d583a-323b-4394-9df3-949a3f713708
title: MFPKEY_VBRQUALITY Property
ms.topic: article
ms.date: 05/31/2018
---

# MFPKEY\_VBRQUALITY Property

Specifies the actual quality level for quality based (1-pass) variable-bit-rate (VBR) encoding.

## Constant for IPropertyBag

g\_wszWMVCVBRQuality, g\_wszWMCPAudioVBRQuality

## Data Type

VT\_I4

## Remarks

Not all of the values in the range have a unique meaning. The values that represent a step up in quality from the previous level are: 1, 4, 8, 11, 15, 18, 22, 25, 29, 33, 36, 40, 43, 47, 50, 54, 58, 61, 65, 68, 72, 75, 79, 83, 86, 90, 93, 97, and 100.

For audio encoder objects, the quality modes are provided in the [**WAVEFORMATEX**](https://msdn.microsoft.com/library/Dd390970(v=VS.85).aspx) structure of the output types that you retrieve using the [**IMediaObject::GetOutputType**](https://msdn.microsoft.com/en-us/library/Dd406956(v=VS.85).aspx).

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                          |
| Minimum supported server<br/> | Windows Server 2008 \[desktop apps only\]<br/>                                    |
| Header<br/>                   | <dl> <dt>Wmcodecdsp.h</dt> </dl> |



## See also

<dl> <dt>

[Enumerating Audio Types for Specific Encoding Modes](enumeratingaudiotypesforspecificencodingmodes.md)
</dt> <dt>

[Media Foundation Properties](media-foundation-properties.md)
</dt> </dl>

 

 




