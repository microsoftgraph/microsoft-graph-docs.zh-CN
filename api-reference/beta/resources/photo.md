---
title: 照片资源类型
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.date: 09/10/2017
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bdb587e7440fd98c48f71a2611e2a34e039367dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521881"
---
# <a name="photo-resource-type"></a>照片资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。

> [!NOTE]
> 目前，只有**takenDateTime**在 OneDrive for Business 和 SharePoint 上可用。

## <a name="properties"></a>属性

| 属性          | 类型          | 说明                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|cameraMake         |String         | 相机制造商。只读。                                            |
|cameraModel        |String         | 相机型号。只读。                                                   |
|exposureDenominator|双精度         | 相机的曝光时间分数的分母。只读。 |
|exposureNumerator  |Double         | 相机的曝光时间分数的分子。只读。   |
|fNumber            |双精度         | 相机的 F-stop 值。只读。                               |
|focalLength        |双精度数         | 相机的焦距。只读。                               |
|iso                |Int32          | 相机的 ISO 值。只读。                                  |
|orientation        |Int16          | 相机中的方向值。 在 OneDrive 个人版上是可写的。      |
|takenDateTime      |DateTimeOffset | 以 UTC 时间拍摄照片的日期和时间。 只读。              |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.photo",
  "baseType": null
}-->

```json
{
  "cameraMake": "String",
  "cameraModel": "String",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The photo resource provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": ""
}-->
