---
title: signInLocation 资源类型
description: 提供发生登录的城市、省/市/自治区和国家/地区。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: eb4208820c1654a5b8db0d4afa2eeb1df4fb2b53
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808590"
---
# <a name="signinlocation-resource-type"></a>signInLocation 资源类型

命名空间： microsoft. graph 提供了发生登录的城市、省/市/自治区和国家/地区。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|城市|String|提供发起登录的城市。 这是通过登录活动中的纬度/经度信息计算得出的。|
|countryOrRegion|String|提供国家/地区代码信息 (2 号代码) 在该登录起源中。  这是通过登录活动中的纬度/经度信息计算得出的。|
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
