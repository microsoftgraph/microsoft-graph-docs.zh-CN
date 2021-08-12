---
title: outlookGeoCoordinates 资源类型
description: 地理坐标、海拔，以及它们物理位置的精确度。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9a7a1a31b15d4d2e4c72b6ab4a269b9b955831acf470dec2000d0ecf6c023e99
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251875"
---
# <a name="outlookgeocoordinates-resource-type"></a>outlookGeoCoordinates 资源类型

命名空间：microsoft.graph

地理坐标、海拔，以及它们物理位置的精确度。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accuracy|double|纬度和经度的精确度。 举个例子，精确度可以以米为单位度量，如纬度和经度可以精确到 50 米内。|
|altitude|double|位置的海拔高度。|
|altitudeAccuracy|double|海拔高度的精确度。|
|latitude|double|位置的纬度。|
|longitude|double|位置的经度。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

