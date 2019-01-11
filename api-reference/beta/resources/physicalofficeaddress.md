---
title: physicalOfficeAddress 资源类型
description: 代表资源如 contact 或事件的业务地址。
localization_priority: Normal
ms.openlocfilehash: bd4274e29b2ef0f9e7e8318528d18103be19fabc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817785"
---
# <a name="physicalofficeaddress-resource-type"></a>physicalOfficeAddress 资源类型

表示业务地址的资源，如组织联系人。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|city|String|城市。|
|countryOrRegion|字符串|国家或地区。它是任意格式的字符串值，例如“United States”。|
|officeLocation  | String | 如构建和 office 号码为组织的联系人的办公室位置。  |
|postalCode|String|邮政编码。|
|state|String|省/市/自治区。|
|street|String|街道。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
