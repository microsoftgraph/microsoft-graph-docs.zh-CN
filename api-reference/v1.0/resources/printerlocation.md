---
title: printerLocation 资源类型
description: 表示打印机的物理和分层位置。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 46e79bd9833f43c7529e77d462822f703cedf9ee
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60942532"
---
# <a name="printerlocation-resource-type"></a>printerLocation 资源类型

命名空间：microsoft.graph

表示打印机的物理和分层位置。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|latitude|Double|打印机所在的纬度。|
|longitude|Double|打印机所在的经度。|
|altitudeInMeters|Int32|打印机所在的高度（以米为单位）。|
|streetAddress|String|打印机所在的街道地址。|
|subUnit|String 集合|打印机所在的次级层次结构。 元素应按层次结构顺序。 例如，如果校园分为不同的分区，则层次结构可能如下所示： `["East Wing", "Block A"]`|
|城市|String|打印机所在的城市。|
|postalCode|String|打印机所在的邮政编码。|
|countryOrRegion|String|打印机所在的国家/地区。|
|网站|String|打印机所在的站点。|
|building|String|打印机所在的建筑物。|
|floor|String|打印机所在的楼层。 目前仅支持数值。|
|floorDescription|String|打印机所在的楼层的说明。|
|roomName|String|打印机所在的房间。 目前仅支持数值。|
|roomDescription|String|打印机所在的房间的说明。|
|组织|String 集合|打印机所属的组织层次结构。 元素应按层次结构顺序。|
|subdivision|String 集合|打印机所在的细分。 元素应按层次结构顺序。|
|stateOrProvince|String|打印机所在的州或省。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerLocation",
  "latitude": "Double",
  "longitude": "Double",
  "altitudeInMeters": "Integer",
  "streetAddress": "String",
  "subunit": [
    "String"
  ],
  "city": "String",
  "postalCode": "String",
  "countryOrRegion": "String",
  "site": "String",
  "building": "String",
  "floor": "String",
  "floorDescription": "String",
  "roomName": "String",
  "roomDescription": "String",
  "organization": [
    "String"
  ],
  "subdivision": [
    "String"
  ],
  "stateOrProvince": "String"
}
```

