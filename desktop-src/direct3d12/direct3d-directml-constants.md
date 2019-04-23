---
title: DirectML constants
description: The following constants are declared in DirectML.h.
keywords:
- Constants
topic_type:
- apiref
api_name:
- DirectML constants
api_location:
- DirectML.h
api_type:
- HeaderDef
ms.topic: article
ms.date: 04/10/2019
ms.custom: 19H1
---

# DirectML constants

The following constants are declared in DirectML.h.

## DML_TENSOR_DIMENSION_COUNT_MAX (5)
DirectML tensors support a maximum of 5 dimensions.

## DML_TEMPORARY_BUFFER_ALIGNMENT (256)
Temporary and persistent buffers must have a base address that is aligned to 256 bytes.

## DML_PERSISTENT_BUFFER_ALIGNMENT (256)
Temporary and persistent buffers must have a base address that is aligned to 256 bytes.

## DML_MINIMUM_BUFFER_TENSOR_ALIGNMENT (16)
Buffer tensors have a minimum base address alignment requirement of 16 bytes.

## Requirements

| | |
|-|-|
| Header | D3D12.h |

## See also

* [DirectML reference](direct3d-directml-reference.md)
* [Core reference](direct3d-12-core-reference.md)
* [Direct3D 12 Reference](direct3d-12-reference.md)