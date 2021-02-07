---
title: signInLocation 资源类型
description: 提供登录发生位置的城市、省/市/自治区和国家/地区。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c003fda44e54bbee5957e794d02b90f008f4b8f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137093"
---
# <a name="signinlocation-resource-type"></a>signInLocation 资源类型

命名空间：microsoft.graph

提供登录发生位置的城市、省/市/自治区和国家/地区。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|城市|String|提供登录来源城市。 这是使用登录活动中的纬度/经度信息计算得出的。|
|countryOrRegion|String|提供登录 (位置) 2 个字母代码的国家/地区代码信息。  这是使用登录活动中的纬度/经度信息计算得出的。|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|提供登录来源的纬度、经度和高度。|
|state|String|提供登录来源的状态。 这是使用登录活动中的纬度/经度信息计算得出的。|

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

