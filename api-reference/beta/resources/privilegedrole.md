---
title: privilegedRole 资源类型
description: 表示 Azure AD 管理员角色，例如：全局管理员、帐单管理员、 **服务管理员、用户管理员、密码管理员** 等。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 4eca2f1a3d9de4fa7f625cd6b559b5a0c9c03916
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444012"
---
# <a name="privilegedrole-resource-type"></a>privilegedRole 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD 管理员角色，例如：全局管理员、帐单管理员、 **服务管理员、用户管理员、密码管理员** 等。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 privilegedRole 对象](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md) 集合|获取 privilegedRole 的集合。|
|[获取 privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |读取 privilegedRole 对象的属性和关系。|
|[列出作业](../api/privilegedrole-list-assignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md) 集合| 获取此角色的分配对象集合。|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|激活分配的角色。|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|停用分配的角色。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string|管理员角色的唯一标识符。 它是一个 GUID 字符串，其值与给定角色的 Azure AD 中的角色模板 ID 相同。 只读。|
|name|string|角色名称。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|assignments|[privilegedRoleAssignment](privilegedroleassignment.md) 集合| 此角色的分配。 只读。 可为 Null。|
|settings|[privilegedRoleSettings](privilegedrolesettings.md)| 此角色的设置。 只读。 可为 NULL。|
|摘要|[privilegedRoleSummary](privilegedrolesummary.md)| 此角色的摘要信息。 只读。 可为 Null。|

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


