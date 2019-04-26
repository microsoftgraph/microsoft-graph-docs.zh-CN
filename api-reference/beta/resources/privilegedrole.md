---
title: privilegedRole 资源类型
description: 表示 Azure AD 管理员角色, 例如:**全局管理员、记帐管理员、服务管理员、用户管理员、密码管理员**等。
localization_priority: Normal
ms.openlocfilehash: 9b5454745257bea071f967b654d3b6174c3c3289
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344270"
---
# <a name="privilegedrole-resource-type"></a>privilegedRole 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD 管理员角色, 例如:**全局管理员、记帐管理员、服务管理员、用户管理员、密码管理员**等。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 privilegedRole 对象](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md) 集合|获取 privilegedRole 的集合。|
|[获取 privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |读取 privilegedRole 对象的属性和关系。|
|[列出作业](../api/privilegedrole-list-assignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md) 集合| 获取此角色的工作分配对象集合。|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|激活分配的角色。|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|停用分配的角色。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string|管理员角色的唯一标识符。 它是一个 GUID 字符串, 与给定角色的 Azure AD 中的角色模板 id 具有相同的值。 只读。|
|name|string|角色名称。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|assignments|[privilegedRoleAssignment](privilegedroleassignment.md) 集合| 此角色的分配。 此为只读属性。 可为 Null。|
|settings|[privilegedRoleSettings](privilegedrolesettings.md)| 此角色的设置。 此为只读属性。 可为 Null。|
|摘要|[privilegedRoleSummary](privilegedrolesummary.md)| 此角色的摘要信息。 此为只读属性。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
