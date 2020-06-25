---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a62a138cbd48645b6b296abcde72af0cef19e259
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863731"
---
# <a name="photo-resource-type"></a>Photo 资源类型

命名空间：microsoft.graph

**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->

```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>属性

| 属性                | 类型           | 说明
|:------------------------|:---------------|:----------------------------------
| **takenDateTime**       | DateTimeOffset | Represents the date and time the photo was taken. Read-only.
| **cameraMake**          | String         | Camera manufacturer. Read-only.
| **cameraModel**         | String         | Camera model. Read-only.
| **fNumber**             | 双精度         | The F-stop value from the camera. Read-only.
| **exposureDenominator** | 双精度         | The denominator for the exposure time fraction from the camera. Read-only.
| **exposureNumerator**   | Double         | The numerator for the exposure time fraction from the camera. Read-only.
| **focalLength**         | 双精度数         | The focal length from the camera. Read-only.
| **iso**                 | Int32          | The ISO value from the camera. Read-only.
| **orientation**         | Int16          | 相机中的方向值。 在 OneDrive 个人版上是可写的。      |

## <a name="remarks"></a>注解

OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。

有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
