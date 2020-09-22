---
title: 会议室资源类型
description: 指定租户中聊天室的属性。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ff64a11b9a4e0e036824df1629f1ae055ade3f9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016133"
---
# <a name="room-resource-type"></a>会议室资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户中的会议室。 

在 Exchange Online 中，每个会议室都与一个会议室邮箱相关联。 从 [原位置](place.md)派生。

## <a name="methods"></a>方法

| 方法                              | 返回类型                  | 说明 |
|:------------------------------------|:-----------------------------|:--------|
| [列表位置](../api/place-list.md) | 所请求的派生类型的[位置](place.md)的集合 | 获取在租户中定义的指定类型的 **位置** 对象的集合。 例如，您可以获取租户中的所有会议室、所有会议室列表或特定会议室列表中的会议室。 |
| [获取位置](../api/place-get.md)    | 所请求的派生类型的 [位置](place.md)            | 获取指定的 **place** 对象（例如会议室）的属性和关系。 |

## <a name="properties"></a>属性

| 属性               | 类型                                              | 说明 |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](physicaladdress.md)             | 会议室的街道地址。 |
| audioDeviceName        | String                                            | 指定会议室中音频设备的名称。 |
| bookingType            | [bookingType](#bookingtype-values)                | 会议室的类型。 可能的值为 `standard` 和 `reserved` 。 |
| 幢               | String                                            | 指定聊天室所在的建筑物名称或楼号。 |
| 能够               | String                                            | 指定会议室的容量。 |
| displayName            | String                                            | 与聊天室关联的名称。 |
| displayDeviceName      | String                                            | 指定聊天室中显示设备的名称。 |
| emailAddress           | String                                            | 聊天室的电子邮件地址。 |
| floorLabel             | String                                            | 指定基底的描述性标签，例如 P。 |
| floorNumber            | Int32                                             | 指定会议室所在的楼层号。 |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | 指定纬度、经度和（可选）海拔坐标中的会议室位置。 |
| id                     | String                                            | 聊天室的唯一标识符。 只读。 |
| isWheelchairAccessible | Boolean                                           | 指定会议室是否 wheelchair 可访问。 |
| label                  | String                                            | 指定聊天室的描述性标签，例如数字或名称。 |
| 昵称               | String                                            | 指定聊天室的昵称，例如 "会议室"。 |
| phone                  | String                                            | 会议室的电话号码。 |
| tags                   | String 集合                                 | 指定会议室的其他功能，例如，视图类型或家具类型等详细信息。 |
| videoDeviceName        | String                                            | 指定聊天室中视频设备的名称。 |

### <a name="bookingtype-values"></a>bookingType 值

| 值    | 说明                                               |
|:---------|:----------------------------------------------------------|
| 普通 | 可以根据此 cmdlet 中的其他设置保留该会议室。 此值为默认值。 |
| 保留 | 会议室仅在首次推出时才可用。 无法保留。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.room",
  "baseType": ""
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "audioDeviceName": "String",
  "bookingType": "String",
  "building": "String",
  "capacity": "String",
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelchairAccessible": true,
  "label": "String",
  "nickname": "String",
  "phone": "String",
  "tags": ["String"],
  "videoDeviceName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "room resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


