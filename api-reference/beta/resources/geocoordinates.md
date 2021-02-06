---
author: JeremyKelley
description: geoCoordinates 资源基于文件中包含的元数据提供位置的地理坐标和提升。
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: e3b0ac4f616afe648b5c30dc9d15978036a7ab80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129420"
---
# <a name="geocoordinates-resource-type"></a>geoCoordinates 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

基于文件中包含的元数据提供位置的地理坐标和提升。
如果 [**driveItem**](driveitem.md) 具有非 null **位置** Facet，则该项表示包含已知位置的文件。

> [!NOTE]
> 更新照片的纬度和经度时，必须 (空白或其他) [](photo.md)照片资源。

## <a name="properties"></a>属性

| 属性  | 类型   | 说明
|:----------|:-------|:--------------------------------------------------------
| 海拔  | Double | 可选。此项高于海平面的高度（以英尺为单位）。只读。
| 纬度  | Double | 可选。 此项的纬度（以十进制表示）。 在 OneDrive 个人上可写。
| longitude | Double | 可选。 此项的经度（以十进制表示）。 在 OneDrive 个人上可写。

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


