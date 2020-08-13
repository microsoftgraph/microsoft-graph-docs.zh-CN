---
author: JeremyKelley
description: GeoCoordinates 资源根据文件中包含的元数据提供位置的地理坐标和仰角。
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 07b0a39155b8c9c4dc02d6cff1e0a93c1a9cd418
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497634"
---
# <a name="geocoordinates-resource-type"></a>geoCoordinates 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

根据文件中包含的元数据提供位置的地理坐标和仰角。
如果[**driveItem**](driveitem.md)具有非 null**位置**facet，则该项目表示一个文件，其中包含一个已知的位置关联。

> [!NOTE]
> 更新照片的纬度和经度时，必须提供[照片](photo.md)资源 (空或其他) 。

## <a name="properties"></a>属性

| 属性  | 类型   | 说明
|:----------|:-------|:--------------------------------------------------------
| 海拔  | Double | 可选。此项高于海平面的高度（以英尺为单位）。只读。
| 纬度  | Double | 可选。 此项的纬度（以十进制表示）。 在 OneDrive 个人版上是可写的。
| longitude | Double | 可选。 此项的经度（以十进制表示）。 在 OneDrive 个人版上是可写的。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": []
}
-->
