---
title: printerLocation 资源类型
description: 表示打印机的物理和分层位置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bfb082571ab1c5ddf2b46a06c6e66b9e31e47309
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664056"
---
# <a name="printerlocation-resource-type"></a>printerLocation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机的物理和分层位置。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|latitude|Double|打印机所在的纬度。|
|longitude|Double|打印机所在的经度。|
|altitudeInMeters|Int32|打印机所在的高度（以米为单位）。|
|streetAddress|String|打印机所在的街道地址。|
|subUnit|String collection|打印机所在的次级层次结构。 元素应按层次结构顺序进行。 例如，如果校园分为不同的部分，则层次结构可能如下所示： `["East Wing", "Block A"]`|
|城市|String|打印机所在的城市。|
|postalCode|String|打印机所在的邮政编码。|
|countryOrRegion|String|打印机所在的国家/地区。|
|网站|String|打印机所在的站点。|
|building|String|打印机所在的大楼。|
|floor|String|打印机所在的楼层。 目前仅支持数值。|
|floorDescription|String|打印机所在的楼层的说明。|
|roomName|String|打印机所在的房间。 目前仅支持数值。|
|roomDescription|String|打印机所在的房间的说明。|
|组织|String collection|打印机所属的组织层次结构。 元素应按层次结构顺序进行。|
|subdivision|String collection|打印机所在的细分。 元素应按层次结构顺序进行。|
|stateOrProvince|String|打印机所在的州或省。|

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
    "floor": "123456",
    "floorDescription": "String",
    "roomName": "123456",
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

