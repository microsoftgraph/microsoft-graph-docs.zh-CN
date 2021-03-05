---
title: administrativeUnit 资源类型
description: 管理单元为用户和组目录对象提供概念容器。
localization_priority: Normal
author: anandyadavMSFT
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5ff1e4a5915487837ab7db25d2acefa3fafb4ad5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448875"
---
# <a name="administrativeunit-resource-type"></a>administrativeUnit 资源类型

命名空间：microsoft.graph

管理单元为用户和组目录对象提供概念容器。 通过使用管理单元，公司管理员可以将管理责任委派给区域管理员或部门管理员，以管理包含在管理单元内或作用域内的用户和组。

来看一个示例。 假设 Contoso Corp 由两个部门（一个"西陆岛"分部和一个"东部经济区"部门）所决定。 Contoso 的目录角色的范围为整个租户。 Contoso 公司管理员 Lee 想要委派管理职责，但将其范围缩小到"西陆岛"部门或"东部经济区"部门。  小王可以创建 *一个"西陆岛"管理单元* ，并可以将所有"西陆"用户放入此管理单元中。  同样，小王可以创建 *一个东部经济区管理单元*。  现在，Lee 可以开始将管理职责委派给其他人，但范围是自己创建的新管理单元。 小王将 Jennifer设置在一个范围为"西陆"管理单元的支持 *人员管理员角色中*。  这允许 Jennifer 重置任何用户的密码，但只有在这些用户位于"西陆岛"管理单元 *中时。*  同样，小王将 Dave 设置在一个用户帐户 *管理员* 角色中，该角色的作用范围是"*东部经济区"管理单元*。  这允许 Dave 更新用户、分配许可证和重置任何用户的密码，但只有在这些用户位于东部行政区管理单元 *中时。* 有关视频概述，请参阅 [Azure Active Directory 管理单元简介](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)。


本主题提供 administrativeUnit 实体公开的已声明属性和导航属性的说明，以及可在 administrativeUnits 资源上调用的操作和函数。


## <a name="methods"></a>Methods

| 方法   | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[创建](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | 创建新的管理单元。|
|[List](../api/administrativeunit-list.md) | [administrativeUnit](administrativeunit.md) 集合 |列出所有 administrativeUnits 的属性。|
|[获取](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |读取特定 administrativeUnit 对象的属性和关系。|
|[更新](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)    |更新 administrativeUnit 对象。 |
|[删除](../api/administrativeunit-delete.md) | 无 |删除 administrativeUnit 对象。 |
|[添加成员](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| 在用户或 (中添加成员) 。|
|[List members](../api/administrativeunit-list-members.md) |[directoryObject](directoryobject.md) 集合| 获取用户和 (组) 列表。|
|[获取成员](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| 获取特定成员。|
|[删除成员](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| 删除成员。|
|[添加作用域角色成员](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 添加作用域角色成员。|
|[列出作用域角色成员](../api/administrativeunit-list-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md) 集合| 获取作用域角色管理员的列表。|
|[获取作用域角色成员](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 获取特定作用域角色成员。|
|[删除作用域角色成员](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 删除作用域角色成员。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|string|管理单元的可选说明。|
|displayName|string|管理单元的显示名称。|
|id|string|管理单元的唯一标识符。 只读。|
|visibility|string|控制管理单元及其成员是隐藏还是公开。 可以设置为或 `HiddenMembership` `Public` 。 如果未设置，默认行为为 Public。 设置为 HiddenMembership 时，只有管理单元的成员才能列出管理单元的其他成员。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|成员|[directoryObject](directoryobject.md) collection|是此管理单元的成员的用户和组。 HTTP 方法：get (list members) ， POST (add members) ， DELETE (remove members) .|
|scopedRoleMembers|[scopedRoleMembership](scopedrolemembership.md) 集合| 此管理单元的作用域角色成员。  HTTP 方法：GET (list scopedRoleMemberships) ， POST (add scopedRoleMembership) ， DELETE (remove scopedRoleMembership) 。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.administrativeUnit"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "visibility": "string"
}

```


## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
