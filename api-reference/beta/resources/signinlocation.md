---
title: signInLocation 资源类型
description: 提供市/县、 状态和国家/地区从其中登录发生。
ms.openlocfilehash: a3d4f6ca5ec18e70960f45a3da1bb06d51ee1e65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045572"
---
# <a name="signinlocation-resource-type"></a>signInLocation 资源类型
提供市/县、 状态和国家/地区从其中登录发生。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|city|字符串|提供登录发起的城市。 这被计算使用登录活动纬度/经度信息。|
|countryOrRegion|字符串|提供的国家/地区代码信息 （2 字母代码） 的登录来源。  这被计算使用登录活动纬度/经度信息。|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|提供、 纬度和海拔高度的登录来源。|
|状态|字符串|提供登录发起的状态。 这被计算使用登录活动纬度/经度信息。|

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