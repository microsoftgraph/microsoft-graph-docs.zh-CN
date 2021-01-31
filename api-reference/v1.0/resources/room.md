---
title: 会议室资源类型
description: 指定租户中聊天室的属性。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1a297888d8b469944b5fdbebaa9948db0ba59c97
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059663"
---
# <a name="room-resource-type"></a>会议室资源类型

命名空间：microsoft.graph

表示租户中的聊天室。 

在 Exchange Online 中，每个会议室都与一个会议室邮箱关联。 派生自 [位置](place.md)。

## <a name="methods"></a>方法

| 方法                              | 返回类型                  | 说明 |
|:------------------------------------|:-----------------------------|:--------|
| [列出位置](../api/place-list.md) | 所请求的派生位置类型 [的集合](place.md) | 获取租户中定义的指定类型的 **place** 对象的集合。 例如，可以获取租户中特定会议室列表中的所有会议室、所有会议室列表或会议室。 |
| [获取位置](../api/place-get.md)    | 请求的派生位置 [类型](place.md)            | 获取指定位置 **对象（如** 聊天室）的属性和关系。 |

## <a name="properties"></a>属性

| 属性               | 类型                                              | 说明 |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](physicaladdress.md)             | 房间的街道地址。 |
| audioDeviceName        | String                                            | 指定会议室中的音频设备的名称。 |
| bookingType            | [bookingType](#bookingtype-values)                | 聊天室的类型。 可能的值是 `standard` ， `reserved` 和 。 |
| building               | String                                            | 指定房间的大楼名称或建筑物编号。 |
| capacity               | Int32                                             | 指定会议室的容量。 |
| displayName            | String                                            | 与聊天室关联的名称。 |
| displayDeviceName      | String                                            | 指定会议室中的显示设备的名称。 |
| emailAddress           | String                                            | 会议室的电子邮件地址。 |
| floorLabel             | String                                            | 指定楼层的描述性标签，例如 P。 |
| floorNumber            | Int32                                             | 指定房间的楼层。 |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | 指定以纬度、经度和（可选）高度坐标表示的会议室位置。 |
| id                     | String                                            | 会议室的唯一标识符。 只读。 |
| isWheelChairAccessible | 布尔                                           | 指定会议室是否可供访问。 |
| label                  | String                                            | 指定会议室的描述性标签，例如数字或名称。 |
| nickname               | String                                            | 指定会议室的昵称，例如"conf room"。 |
| phone                  | String                                            | 会议室的电话号码。 |
| tags                   | 字符串集合                                 | 指定会议室的其他功能，例如，视图类型或费用类型等详细信息。 |
| videoDeviceName        | String                                            | 指定会议室中的视频设备的名称。 |

### <a name="bookingtype-values"></a>bookingType 值

| 值    | 说明                                               |
|:---------|:----------------------------------------------------------|
| standard | 会议室可用，可以预订。 此值为默认值。 |
| 保留 | 会议室仅在"先到先得"的基础上可用。 不能保留。|

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
  "capacity": 1024,
  "displayName": "String",
  "displayDeviceName": "String",
  "emailAddress": "String",
  "floorLabel": "String",
  "floorNumber": 1024,
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "isWheelChairAccessible": true,
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

