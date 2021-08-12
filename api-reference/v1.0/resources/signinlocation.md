---
title: signInLocation 资源类型
description: 提供发生登录的城市、省/市/自治区和国家/地区。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fb22cf430ec3bffd04150398600beae5af4c41579f00f3cf49196587efb9f44b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124155"
---
# <a name="signinlocation-resource-type"></a>signInLocation 资源类型

命名空间：microsoft.graph

提供发生登录的城市、省/市/自治区和国家/地区。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|城市|String|提供登录的来源城市。 这是使用登录活动中的经纬度信息计算的。|
|countryOrRegion|String|提供登录来源 (2 个字母) 代码的国家/地区代码信息。  这是使用登录活动中的经纬度信息计算的。|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|提供登录来源的纬度、经度和海拔高度。|
|state|String|提供登录来源的状态。 这是使用登录活动中的经纬度信息计算的。|

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

