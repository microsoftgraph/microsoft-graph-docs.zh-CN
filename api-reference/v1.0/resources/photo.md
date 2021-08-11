---
author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1f2d69159ba7a054ca821f00f56dfa7627b4422d6069708eaa6ad8f53de651e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196843"
---
# <a name="photo-resource-type"></a>Photo 资源类型

命名空间：microsoft.graph

**照片** 资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。

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
| **takenDateTime**       | DateTimeOffset | 表示照片拍摄的时间和日期。只读。
| **cameraMake**          | String         | 相机制造商。只读。
| **cameraModel**         | String         | 相机型号。只读。
| **fNumber**             | Double         | 相机的 F-stop 值。只读。
| **exposureDenominator** | Double         | 相机的曝光时间分数的分母。只读。
| **exposureNumerator**   | Double         | 相机的曝光时间分数的分子。只读。
| **focalLength**         | Double         | 相机的焦距。只读。
| **iso**                 | Int32          | 相机的 ISO 值。只读。
| **orientation**         | Int16          | 相机的方向值。 可写OneDrive个人。      |

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

