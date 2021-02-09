---
title: place 资源类型
description: 表示位置。 这是会议室或 roomList 的基本类型。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8b9f7d21212c6551201b7ce83ba6c8f11edffa98
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161129"
---
# <a name="place-resource-type"></a>place 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示基本的位置属性，如名称、物理地址和地理坐标。 这是更丰富的位置类型（如 room 和[](room.md) [roomList）的基本类型](roomlist.md)。

### <a name="using-the-places-api"></a>使用位置 API
Exchange Online 管理员可以将租户中的会议室组织到会议室列表中。 使用位置 API，可以获取租户中所有会议室列表或会议室，或获取特定会议室列表中的所有会议室。

会议室 [和 roomList](room.md)等位置包含基本 [](roomlist.md)**id、显示名称** 和电子邮件地址。 此外，它们包含导航信息（如物理地址和地理坐标）以及房间信息、其他相关信息（如 AV 功能、楼层和容量）。

[findRooms 和](../api/user-findrooms.md) [findRoomLists](../api/user-findroomlists.md)函数支持对租户中的会议室和会议室列表进行类似的查找。 下面是位置 API 和这些函数之间的比较。  如果要创建生产应用，请选择位置 API，因为 API 现已在 v1.0 中普遍提供。 计划更新使用 **findRooms** 或 **findRoomLists** 使用位置 API 的任何现有代码，因为 **findRooms** 或 **findRoomLists** 将弃用，并且将公布时间线。

|Places API |findRooms 和 findRoomLists 函数|
|:------------------------------------|:-----------------------------|
|支持获取租户中所有会议室或会议室列表，以及会议室列表中的所有会议室 | 类似支持 - 获取租户中所有会议室或会议室列表，以及会议室列表中的所有会议室|
|[列出位置](../api/place-list.md) 可以返回租户中的 100 多个会议室 | [findRooms](../api/user-findrooms.md) 最多返回租户中的前 100 个会议室 |
|支持 [获取租户中的单个会议室](../api/place-get.md) 或会议室列表 | 不支持获取租户中的单个会议室或会议室列表
|定义会议室和[roomList](roomlist.md) [](room.md)的特定实体，这些实体指定更丰富的属性集，以及显示名称 SMTP 地址。 | 每个会议室和会议室列表都是一种轻型 [电子邮件](emailaddress.md) 地址类型，它仅指定显示名称 SMTP 地址|
|仅支持具有委派工作 (学校帐户或) 或应用程序权限的组织方案 | 仅对具有委派权限或应用程序权限的组织方案的类似支持|
|支持 [更新租户中的单个会议室](../api/place-update.md) 或会议室列表 | 不支持更新租户中的单个会议室或会议室列表

## <a name="methods"></a>方法

| 方法                              | 返回类型                  | 说明 |
|:------------------------------------|:-----------------------------|:--------|
| [列出位置](../api/place-list.md) | 所请求的派生位置类型 [的集合](place.md) | 获取租户中定义的指定类型的 **place** 对象的集合。 |
| [获取位置](../api/place-get.md)    | 请求的派生位置 [类型](place.md)            | 获取指定 place 对象 **的属性和** 关系。 |
| [更新位置](../api/place-update.md)    | 请求的派生位置 [类型](place.md)            | 更新指定 place 对象 **的属性和** 关系。 |

## <a name="properties"></a>属性

| 属性       | 类型                                              | 说明 |
|:---------------|:--------------------------------------------------|:--------|
| address        | [physicalAddress](physicaladdress.md)             | 位置的街道地址。 |
| displayName    | String                                            | 与位置关联的名称。 |
| geoCoordinates | [outlookGeoCoordinates](outlookgeocoordinates.md) | 指定以纬度、经度和纬度（可选） (高度坐标) 位置。 |
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
- 若要使管理员创建会议室列表，请使用 Exchange PowerShell cmdlet [New-DistributionGroup。](/powershell/module/exchange/users-and-groups/new-distributiongroup)
- 对于将会议室添加到会议室列表的管理员，请使用 Exchange Powershell cmdlet [Add-DistributionGroupMember。](/powershell/module/exchange/users-and-groups/add-distributiongroupmember)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "place resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
