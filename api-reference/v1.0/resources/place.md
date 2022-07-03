---
title: 放置资源类型
description: 表示一个位置。 这是会议室或会议室列表的基类型。
ms.localizationpriority: medium
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8469be739bdf645e0d588af33918c5c51aecd3bf
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609715"
---
# <a name="place-resource-type"></a>放置资源类型

命名空间：microsoft.graph

表示基本位置属性，例如名称、物理地址和地理坐标。 这是更丰富的位置类型的基类型，如 [room](room.md) 和 [roomList](roomlist.md)。

### <a name="using-the-places-api"></a>使用位置 API
Exchange Online管理员可以将租户中的会议室组织到会议室列表中。 使用位置 API，可以获取租户中的所有会议室列表或会议室，或获取特定会议室列表中的所有会议室。

[会议室](room.md)和 [会议室列表](roomlist.md)等位置包含基本 **ID**、显示名称和电子邮件地址。 此外，它们还包含导航信息，如物理地址和地理坐标，以及房间中的其他相关信息，如 AV 功能、楼层数和容量。

[findRooms](/graph/api/user-findrooms) 和 [findRoomLists 函](/graph/api/user-findroomlists)数支持对租户中的会议室和会议室列表进行类似的查找。 下面是位置 API 与这些函数之间的比较。  如果要创建生产应用，请选择 API 的位置，因为 API 现已在 v1.0 中正式发布。 计划更新使用 **findRooms** 或 **findRoomLists** 来使用位置 API 的任何现有代码，因为 **findRooms** 或 **findRoomLists** 将被弃用，并且将宣布一个时间线。

|放置 API |findRooms 和 findRoomLists 函数|
|:------------------------------------|:-----------------------------|
|支持获取租户中的所有会议室或会议室列表，以及会议室列表中的所有会议室 | 类似的支持 - 获取租户中的所有会议室或会议室列表，以及会议室列表中的所有会议室|
|[列表位置](../api/place-list.md) 可以返回租户中的 100 多个房间 | [findRooms](/graph/api/user-findrooms) 返回租户中前 100 个房间 |
|支持在租户中[获取单个会议室或会议室列表](../api/place-get.md) | 不支持在租户中获取单个会议室或会议室列表
|定义 [会议室](room.md) 和 [roomList](roomlist.md) 的特定实体，除了显示名称和 SMTP 地址外，还指定更丰富的属性集。 | 每个会议室和会议室列表都具有较轻的权重 [emailAddress](emailaddress.md) 类型，仅指定显示名称和 SMTP 地址|
|仅支持具有委派 (工作或学校帐户) 或应用程序权限的组织方案 | 仅对具有委派权限或应用程序权限的组织方案的类似支持|
|支持更新租户中的[单个会议室或会议室列表](../api/place-update.md) | 不支持更新租户中的单个会议室或会议室列表

## <a name="methods"></a>方法

| 方法                              | 返回类型                  | 说明 |
|:------------------------------------|:-----------------------------|:--------|
| [列出位置](../api/place-list.md) | 请求的派生[位置](place.md)类型的集合 | 获取租户中定义的指定类型的 **位置** 对象的集合。 |
| [获取位置](../api/place-get.md)    | 请求的派生[位置](place.md)类型            | 获取指定 **位置** 对象的属性和关系。 |
| [更新位置](../api/place-update.md)    | 请求的派生[位置](place.md)类型            | 更新指定 **位置** 对象的属性和关系。 |

## <a name="properties"></a>属性

| 属性       | 类型                                              | 说明 |
|:---------------|:--------------------------------------------------|:--------|
| address        | [physicalAddress](physicaladdress.md)             | 地点的街道地址。 |
| displayName    | String                                            | 与该位置关联的名称。 |
| geoCoordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | 指定纬度、经度和 (（可选）) 海拔坐标的位置。 |
| id             | String                                            | 位置的唯一标识符。 只读。 |
| phone          | String                                            | 位置的电话号码。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.place"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "String",
  "id": "String (identifier)",
  "geoCoordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "phone": "String"
}
```

## <a name="see-also"></a>另请参阅
- 若要让管理员创建会议室列表，请使用 Exchange PowerShell cmdlet [New-DistributionGroup](/powershell/module/exchange/users-and-groups/new-distributiongroup?view=exchange-ps&preserve-view=true)。
- 若要让管理员将会议室添加到会议室列表，请使用 Exchange Powershell cmdlet [Add-DistributionGroupMember](/powershell/module/exchange/users-and-groups/add-distributiongroupmember?view=exchange-ps&preserve-view=true)。

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
