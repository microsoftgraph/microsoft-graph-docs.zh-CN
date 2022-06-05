---
title: physicalAddress 资源类型
description: 表示资源（例如联系人或事件）的街道地址。
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 44ee09d7f02614c7fc7fc6afd8ef88a79f557369
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898138"
---
# <a name="physicaladdress-resource-type"></a>physicalAddress 资源类型

命名空间：microsoft.graph

表示资源（例如联系人或事件）的街道地址。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|城市|String|城市。|
|countryOrRegion|String|国家或地区。它是任意格式的字符串值，例如“United States”。|
|postalCode|String|邮政编码。|
|state|String|省/市/自治区。|
|street|String|街道。|

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
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

