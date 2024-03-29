---
title: administrativeUnit 资源类型
description: 管理单元为用户和组目录对象提供概念容器。
ms.localizationpriority: medium
author: DougKirschner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 702ff256e52721af990ee0fc211b4178dc0ad972
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555497"
---
# <a name="administrativeunit-resource-type"></a>administrativeUnit 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

管理单元为用户、组和设备目录对象提供概念容器。 使用管理单位，公司管理员现在可以将管理职责委托给区域或部门管理员，以管理包含在管理单元内或范围内的用户、组和设备。 此资源是允许传入其他属性的开放类型。

该资源支持通过提供 [delta](../api/administrativeunit-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。 

来看一个示例。 想象一下，Contoso 公司由两个部门组成——一个西海岸司和一个东海岸司。 Contoso 中的目录角色的范围限于整个租户。 Contoso 公司管理员 Lee 希望委派管理职责，但将其范围限定在西海岸司或东海岸部门。  Lee 可以创建 *一个西海岸辅助单元* ，并将所有西海岸用户置于此管理单元中。  同样，Lee 可以创建 *东海岸管理单元*。  现在，李先生可以开始将行政职责委托给他人，但 **范围限于** 他创建的新行政单位。 李将詹妮弗置于一个 *支持管理员* 角色 **中，该角色的范围限于***西海岸行政部门*。  这允许 Jennifer 重置任何用户的密码，但前提是这些用户位于 *西海岸管理单元* 中。  同样，Lee 将 Dave 置于一个用户 *帐户管理员* 角色 **中，该角色的范围限于***东海岸管理单元*。  这允许 Dave 更新用户、分配许可证和重置任何用户的密码，但前提是这些用户位于 *东海岸管理单元* 中。 有关视频概述，请参阅 [Azure Active Directory 管理单元简介](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)。

该资源支持：

- 将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。
- 通过提供 [delta](../api/user-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。


## <a name="methods"></a>方法

| 方法   | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[创建](../api/directory-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | 创建新的管理单元。|
|[列表](../api/directory-list-administrativeunits.md) | [administrativeUnit](administrativeunit.md) 集合 |列出所有 administrativeUnits 的属性。|
|[Get](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |读取特定 administrativeUnit 对象的属性和关系。|
|[更新](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)    |更新 administrativeUnit 对象。 |
|[删除](../api/administrativeunit-delete.md) | None |删除 administrativeUnit 对象。 |
|[获取增量](../api/administrativeunit-delta.md)|[administrativeUnit](administrativeunit.md)|获取新创建、更新或删除的 **administrativeUnits** ，而无需对整个资源集合执行完整读取。|
|[添加成员](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| 添加成员 (用户或组) 。|
|[List members](../api/administrativeunit-list-members.md) |[directoryObject](directoryobject.md) 集合| 获取 (用户和组) 成员的列表。|
|[获取成员](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| 获取特定成员。|
|[删除成员](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| 删除成员。|
|[添加 scopedRoleMember](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 分配具有管理单元范围的 Azure AD 角色。|
|[列出 scopedRoleMembers](../api/administrativeunit-list-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md) 集合| 列出具有管理单元范围的 Azure AD 角色分配。|
|[获取 scopedRoleMember](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 获取具有管理单元范围的 Azure AD 角色分配。|
|[删除 scopedRoleMember](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| 删除具有管理单元范围的 Azure AD 角色分配。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|

> [!NOTE]
> 用于调用 **administrativeUnits** API `/administrativeUnits` 的 URL 终结点位于 `beta` 终结点中，但在 `/directory/administrativeUnits` 终结点中 `v1.0` 。

## <a name="properties"></a>属性

> [!IMPORTANT]
> 仅当使用设置为 `eventual` 和 `$count` 的 **ConsistencyLevel** 标头时，才支持 `$filter` 和 `$search` 查询参数的特定用法。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries#administrative-unit-properties)。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|字符串|管理单元的可选说明。 支持`$filter` (`eq`、`ne`、 `in``startsWith`) 、 `$search`|
|displayName|String|管理单元的显示名称。 支持 `$filter` (`eq`、`ne`、`not`、`ge`、`le`、`in`、`startsWith` 和 `null` 值上的 `eq`)、`$search` 和 `$orderBy`。|
|id|String|管理单元的唯一标识符。 只读。 支持 `$filter`（`eq`）。|
| membershipRule | String | 管理单元的动态成员身份规则。 有关可用于动态管理单元和动态组的规则的详细信息，请 [参阅使用属性创建高级规则](https://azure.microsoft.com/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/)。 |
| membershipRuleProcessingState | String | 用于控制是否主动处理动态成员身份规则。 设置为 `On` 希望动态成员身份规则处于活动状态，以及 `Paused` 是否要停止动态更新成员身份。 如果未设置，则默认行为为 `Paused`。 |
| membershipType | String | 管理单元的成员身份类型。 可以是 `dynamic` 或 `assigned`. 如果未设置，则默认行为为 `assigned`。 |
| visibility | String | 控制管理单元及其成员是隐藏的还是公开的。 可以设置为 `HiddenMembership` 或 `Public`. 如果未设置，则默认行为为 `Public`。 设置为 `HiddenMembership`后，只有管理单位的成员才能列出管理单位的其他成员。 |

> [!TIP]
> 默认情况下，目录扩展和关联数据返回，而架构扩展和关联数据仅 `$select`返回。

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|extensions|[扩展](extension.md)集合|为此管理单元定义的开放扩展的集合。 可为 Null。|
|members|[directoryObject](directoryobject.md) collection|属于此管理单元成员的用户和组。 支持 `$expand`。|
|scopedRoleMembers|[scopedRoleMembership](scopedrolemembership.md) 集合| 此管理单元的作用域角色成员。|

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
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "visibility": "String",
  "membershipType": "String",
  "membershipRule": "String",
  "membershipRuleProcessingState": "String"
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


