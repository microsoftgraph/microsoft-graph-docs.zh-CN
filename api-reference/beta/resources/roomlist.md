---
title: roomList 资源类型
description: 代表由公司创建的一组聊天室。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f0c56f986663c71d8c6817c0024919e8714af94a
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841253"
---
# <a name="roomlist-resource-type"></a>roomList 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在租户中定义的一组[聊天室](room.md)对象。

从[原位置](place.md)派生。

## <a name="methods"></a>方法

| 方法                              | 返回类型                  | 说明 |
|:------------------------------------|:-----------------------------|:--------|
| [列表位置](../api/place-list.md) | 所请求的派生类型的[位置](place.md)的集合 | 获取在租户中定义的指定类型的**位置**对象的集合。 例如, 您可以获取租户中的所有会议室、所有会议室列表或特定会议室列表中的会议室。|
| [获取位置](../api/place-get.md)    | 所请求的派生类型的[位置](place.md)            | 获取指定的**place**对象的属性和关系, 如会议室列表。 |

## <a name="properties"></a>属性

| 属性       | 类型                                              | 说明 |
|:---------------|:--------------------------------------------------|:--------|
| address        | [physicalAddress](physicaladdress.md)             | 会议室列表的街道地址。 |
| displayName    | 字符串                                            | 与会议室列表关联的名称。 |
| emailAddress   | String                                            | 会议室列表的电子邮件地址。 |
| geoCoordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | 指定纬度、经度和 (可选) 海拔高度坐标中的 roomlist 位置。 |
| id             | String                                            | 会议室列表的唯一标识符。 只读。 |
| phone          | String                                            | 会议室列表的电话号码。 |

## <a name="relationships"></a>关系

| 关系 | 类型                         | 说明          |
|:-------------|:-----------------------------|:---------------------|
| 所属        | [place](place.md)集合 | 只读。可为空。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.roomList"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "emailAddress": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "id": "String (identifier)",
  "phone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roomList resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
