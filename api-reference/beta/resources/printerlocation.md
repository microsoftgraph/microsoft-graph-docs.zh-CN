---
title: printerLocation 资源类型
description: 表示打印机的物理和分层位置。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 53eeee6e135276ff43e5cd360fbc6615d2df649f
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176609"
---
# <a name="printerlocation-resource-type"></a>printerLocation 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机的物理和分层位置。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|latitude|Double|打印机所在的纬度。|
|longitude|Double|打印机所在的经度。|
|altitudeInMeters|Int32|打印机所在的海拔高度（以米为单位）。|
|streetAddress|String|打印机所在的街道地址。|
|亚基|String collection|打印机所在的子单元层次结构。 元素应按分层顺序排列。 例如，如果一个校园划分为不同的部分，层次结构可能如下所示： `["East Wing", "Block A"]`|
|城市|String|打印机所在的城市。|
|postalCode|String|打印机所在的邮政编码。|
|countryOrRegion|String|打印机所在的国家或地区。|
|网站|字符串|打印机所在的网站。|
|建筑|字符串|打印机所在的建筑物。|
|floor|字符串|打印机所在的楼层。 目前仅支持数值。|
|floorDescription|字符串|打印机所在的楼层的说明。|
|roomName|字符串|打印机所在的房间。 目前仅支持数值。|
|roomDescription|String|打印机所在的房间的说明。|
|组织|字符串集合|打印机所属的组织层次结构。 元素应按分层顺序排列。|
|细分|String collection|打印机所在的细分。 元素应按分层顺序排列。|
|stateOrProvince|字符串|打印机所在的州或省。|

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

