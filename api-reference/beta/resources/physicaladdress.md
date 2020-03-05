---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 53b1e18bd1e7b78e7afb479cac3c5f6cc7ecff88
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521874"
---
# <a name="physicaladdress-resource-type"></a>physicalAddress 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示资源（例如联系人或事件）的街道地址。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|城市|String|城市。|
|countryOrRegion|字符串|国家或地区。它是任意格式的字符串值，例如“United States”。|
|postalCode|String|邮政编码。|
|postOfficeBox|String|邮局编号。|
|state|String|省/市/自治区。|
|street|String|街道。|
|type|： Physicaladdresstype|地址类型。 可取值为：`unknown`、`home`、`business`、`other`。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "postOfficeBox": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
