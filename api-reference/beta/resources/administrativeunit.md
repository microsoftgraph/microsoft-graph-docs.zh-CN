---
title: administrativeUnit 资源类型
description: 管理单元为用户和组目录对象提供概念容器。
ms.localizationpriority: medium
author: DougKirschner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 1dc8844506a7610f6f52b84cfc8abaf4f00d7182
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322119"
---
# <a name="administrativeunit-resource-type"></a>administrativeUnit 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

管理单元为用户和组目录对象提供概念容器。 通过使用管理单元，公司管理员现在可以将管理责任委派给区域管理员或部门管理员，以管理管理单元中包含的用户和组或范围所包含的用户和组。

该资源支持通过提供 [delta](../api/administrativeunit-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。 此资源是允许传入其他属性的开放类型。

来看一个示例。 Imagine Contoso Corp 由两个部门（一个东海岸分部和一个东海岸部门）所决定。 Contoso 的目录角色的范围为整个租户。 Contoso 公司管理员 Lee 希望委派管理责任，但将其范围划分到东海岸部门或东海岸分部。  Lee 可以创建 *一个"东海岸* "管理单元，并可以将所有"东海岸"用户放入此管理单元中。  同样，Lee 可以创建一 *个"东海岸管理单元"。*  现在，Lee 可以开始将管理职责委派给其他人，但作用域为自己创建的新管理单元。 Lee 将 Jennifer 设置在一个支持 *人员管理员* 角色 **中** ，该角色的作用范围为 *"东海岸"管理单元*。  这允许 Jennifer 重置任何用户的密码，但只有在这些用户位于东海岸管理 *单元时。*  同样，Lee 将 Dave 设置在 *一个用户帐户管理员* 角色中，该角色的作用范围为"*东海岸"管理单元*。   这允许 Dave 更新用户、分配许可证和重置任何用户的密码，但只有在这些用户位于东海岸管理 *单元中时。* 有关视频概述，请参阅管理单元[Azure Active Directory简介](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)。

使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。

本主题提供 administrativeUnit 实体公开的已声明属性和导航属性的说明，以及可在 administrativeUnits 资源上调用的操作和函数。


## <a name="methods"></a>Methods

| 方法   | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[创建](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | 创建新的管理单元。|
|[List](../api/administrativeunit-list.md) | [administrativeUnit](administrativeunit.md) 集合 |列出所有 administrativeUnits 的属性。|
|[获取](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |读取特定 administrativeUnit 对象的属性和关系。|
|[更新](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)    |更新 administrativeUnit 对象。 |
|[删除](../api/administrativeunit-delete.md) | 无 |删除 administrativeUnit 对象。 |
|[Get delta](../api/administrativeunit-delta.md)|[administrativeUnit](administrativeunit.md)|获取新创建、更新或删除 **的管理单元** ，而无需执行整个资源集合的完全读取。|
|[添加成员](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| 向用户 (组添加成员) 。|
|[List members](../api/administrativeunit-list-members.md) |[directoryObject](directoryobject.md) 集合| 获取用户和 (组) 列表。|
|[获取成员](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| 获取特定成员。|
|[删除成员](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| 删除成员。|
|[添加作用域角色成员](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 添加作用域角色成员。|
|[列出作用域角色成员](../api/administrativeunit-list-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md) 集合| 获取作用域角色管理员列表。|
|[获取作用域角色成员](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 获取特定作用域角色成员。|
|[删除作用域角色成员](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 删除作用域角色成员。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|

## <a name="properties"></a>属性

> [!IMPORTANT]
> 仅当使用设置为 `eventual` 和 `$count` 的 **ConsistencyLevel** 标头时，才支持 `$filter` 和 `$search` 查询参数的特定用法。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries#administrative-unit-properties)。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|string|管理单元的可选说明。 支持 `$filter`（`eq`、`ne`、`in`、`startsWith`）。|
|displayName|string|管理单元的显示名称。 支持 `$filter` (`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`)、`$search` 和 `$orderBy`。|
|id|string|管理单元的唯一标识符。 只读。 支持 `$filter`（`eq`）。|
|visibility|string|控制管理单元及其成员是隐藏的还是公开的。 可以设置为 `HiddenMembership` 或 `Public` 。 如果未设置，默认行为为 `Public` 。 设置为 `HiddenMembership` 时，只有管理单元的成员可以列出该管理单元的其他成员。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|extensions|[扩展](extension.md)集合|为此管理单元定义的开放扩展集合。 可为 Null。|
|members|[directoryObject](directoryobject.md) 集合|是此管理单元的成员的用户和组。 HTTP 方法：GET (list members) 、POST (add members) 、DELETE (remove members) 。|
|scopedRoleMembers|[scopedRoleMembership](scopedrolemembership.md) 集合| 此管理单元的 Scoped-role 成员。  HTTP 方法：GET (list scopedRoleMemberships) ，POST (add scopedRoleMembership) ， DELETE (remove scopedRoleMembership) . |

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


