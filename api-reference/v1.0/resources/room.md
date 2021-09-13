---
title: 会议室资源类型
description: 指定租户中聊天室的属性。
ms.localizationpriority: medium
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d676dbcd36760bc14edb38b35f6f93573f03b9b5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117772"
---
# <a name="room-resource-type"></a>会议室资源类型

命名空间：microsoft.graph

表示租户中的聊天室。 

在Exchange Online中，每个会议室都与一个会议室邮箱关联。 派生自 [位置](place.md)。

## <a name="methods"></a>方法

| 方法                              | 返回类型                  | 说明 |
|:------------------------------------|:-----------------------------|:--------|
| [列出位置](../api/place-list.md) | 所请求的派生位置类型 [的集合](place.md) | 获取租户中定义的指定 **类型 place** 对象的集合。 例如，可以获取租户中所有会议室、所有会议室列表或特定会议室列表中的会议室。 |
| [获取位置](../api/place-get.md)    | 请求的派生位置 [类型](place.md)            | 获取指定 place **对象（如** 聊天室）的属性和关系。 |

## <a name="properties"></a>属性

| 属性               | 类型                                              | 说明 |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](physicaladdress.md)             | 房间的街道地址。 |
| audioDeviceName        | String                                            | 指定会议室中的音频设备的名称。 |
| bookingType            | [bookingType](#bookingtype-values)                | 聊天室的类型。 可能的值为 、 `standard` 和 `reserved` 。 |
| building               | String                                            | 指定会议室的大楼名称或建筑物编号。 |
| capacity               | Int32                                             | 指定会议室的容量。 |
| displayName            | String                                            | 与会议室关联的名称。 |
| displayDeviceName      | String                                            | 指定会议室中显示设备的名称。 |
| emailAddress           | String                                            | 会议室的电子邮件地址。 |
| floorLabel             | String                                            | 指定楼层的描述性标签，例如 P。 |
| floorNumber            | Int32                                             | 指定房间的楼层。 |
| geoCoordinates         | [outlookGeoCoordinates](outlookgeocoordinates.md) | 指定以纬度、经度和（可选）海拔坐标表示的会议室位置。 |
| id                     | String                                            | 会议室的唯一标识符。 只读。 |
| isWheelChairAccessible | 布尔值                                           | 指定会议室是否可供访问。 |
| 标签                  | String                                            | 指定会议室的描述性标签，例如数字或名称。 |
| nickname               | String                                            | 为会议室指定昵称，例如"conf room"。 |
| phone                  | String                                            | 会议室的电话号码。 |
| 标记                   | 字符串集合                                 | 指定会议室的其他功能，例如，视图类型或装饰类型等详细信息。 |
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
  "@odata.type": "microsoft.graph.room"
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

