---
title: printerLocation 资源类型
description: 表示打印机的物理和分层位置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b8fd40de56d97f70a6208cf68a56c74d711eb78e
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44251091"
---
# <a name="printerlocation-resource-type"></a>printerLocation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机的物理和分层位置。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|latitude|双精度|打印机所在的纬度。|
|longitude|Double|打印机所在的经度。|
|altitudeInMeters|Int32|打印机所在的海拔高度（以米为单位）。|
|streetAddress|String|打印机所在的街道地址。|
|子|String collection|打印机所在的次级单位层次结构。 元素应按层次结构顺序排列。 例如，如果一个校园分成不同的部分，则层次结构可能如下所示：`["East Wing", "Block A"]`|
|city|String|打印机所在的城市。|
|postalCode|String|打印机所在的邮政编码。|
|countryOrRegion|String|打印机所在的国家或地区。|
|网站|String|打印机所在的网站。|
|幢|String|打印机所在的建筑物。|
|floorNumber|Int32|打印机所在的楼层号。|
|floorDescription|String|打印机所在楼层的说明。|
|roomNumber|Int32|打印机所在的房间号码。|
|roomDescription|String|打印机所在聊天室的说明。|
|组织|String collection|打印机所属的组织层次结构。 元素应按层次结构顺序排列。|
|细分|String collection|打印机所在的细分。 元素应按层次结构顺序排列。|
|stateOrProvince|String|打印机所在的省/市/自治区。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerLocation"
}-->

```json
{
    "latitude": 80.1,
    "longitude": -170.1,
    "altitudeInMeters": 123456,
    "streetAddress": "String",
    "subUnit": ["String"],
    "city": "String",
    "postalCode": "String",
    "countryOrRegion": "String",
    "site": "String",
    "building": "String",
    "floorNumber": 123456,
    "floorDescription": "String",
    "roomNumber": 123456,
    "roomDescription": "String",
    "organization": ["String"],
    "subdivision": ["String"],
    "stateOrProvince": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->