---
title: signInLocation 资源类型
description: 提供发生登录的城市、省/市/自治区和国家/地区。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bf0cdec3a2c5feae1b178fc92d02e433d87737a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965024"
---
# <a name="signinlocation-resource-type"></a>signInLocation 资源类型
提供发生登录的城市、省/市/自治区和国家/地区。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|city|String|提供发起登录的城市。 这是通过登录活动中的纬度/经度信息计算得出的。|
|countryOrRegion|String|提供登录所源于的国家/地区代码信息 (2 个字母代码)。  这是通过登录活动中的纬度/经度信息计算得出的。|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|提供登录所源于的纬度、经度和海拔高度。|
|state|String|提供登录的起始状态。 这是通过登录活动中的纬度/经度信息计算得出的。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
