---
title: 照片资源类型
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.date: 09/10/2017
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: bc253cd90a75438f627cf00c55551cfb8bc12d01
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176357"
---
# <a name="photo-resource-type"></a>照片资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**照片** 资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。

> [!NOTE]
> 目前，OneDrive for Business和SharePoint上仅提供 **takenDateTime**。

## <a name="properties"></a>属性

| 属性          | 类型          | Description                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|cameraMake         |String         | 相机制造商。只读。                                            |
|cameraModel        |String         | 相机型号。只读。                                                   |
|exposureDenominator|Double         | 相机的曝光时间分数的分母。只读。 |
|exposureNumerator  |Double         | 相机的曝光时间分数的分子。只读。   |
|fNumber            |Double         | 相机的 F-stop 值。只读。                               |
|focalLength        |Double         | 相机的焦距。只读。                               |
|iso                |Int32          | 相机的 ISO 值。只读。                                  |
|orientation        |Int16          | 相机的方向值。 可在OneDrive个人版上写入。      |
|takenDateTime      |DateTimeOffset | 照片在 UTC 时间拍摄的日期和时间。 只读。              |

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


