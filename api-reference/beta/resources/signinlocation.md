---
title: signInLocation 资源类型
description: 提供发生登录的城市、省/市/自治区和国家/地区。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: fbe356cf939236e1965a2a7005d791bc3a814acc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520581"
---
# <a name="signinlocation-resource-type"></a>signInLocation 资源类型

命名空间： microsoft. graph 提供了发生登录的城市、省/市/自治区和国家/地区。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|城市|String|提供发起登录的城市。 这是通过登录活动中的纬度/经度信息计算得出的。|
|countryOrRegion|String|提供登录所源于的国家/地区代码信息（2个字母代码）。  这是通过登录活动中的纬度/经度信息计算得出的。|
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
