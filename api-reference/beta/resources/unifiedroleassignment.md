---
title: unifiedRoleAssignment 资源类型
description: 角色分配是角色定义和特定作用域的主体之间的链接，目的是为了授予访问权限。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76055128876ab2c4340b55c43c4065f3aac73e4d
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160231"
---
# <a name="unifiedroleassignment-resource-type"></a>unifiedRoleAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

UnifiedRoleAssignment 用于授予对资源的访问权限。 它表示分配给特定范围内的主体（通常为用户）的角色定义。

提供 directoryScopeId 或 appScopeId 是必需的。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 unifiedRoleAssignment](../api/unifiedroleassignment-get.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | 读取 unifiedRoleAssignment 对象的属性和关系。 |
| [创建 unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | 通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignment。 |
| [删除 unifiedRoleAssignment](../api/unifiedroleassignment-delete.md) | 无 | 删除 unifiedRoleAssignment 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| UnifiedRoleAssignment 的唯一标识符。 键，不可为 null，只读。 |
|roleDefinitionId|String| 工作分配所针对的 unifiedRoleDefinition 的 ID。 只读。 |
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|指示工作分配所针对的 roleDefinition 的属性。 提供，以便呼叫者可以在获取角色分配`$expand`的同时使用该角色定义。 roleDefinition.Id 将自动展开
|principalId|String| 向其授予分配的主体的 Objectid。 |
|作主|[directoryObject](directoryobject.md)| 引用分配的主体的属性。 提供，以便呼叫者可以在获取角色`$expand`分配的同时使用。 只读。 |
|directoryScopeId|String|表示工作分配范围的目录对象的 Id。 工作分配的范围决定了主体已被授予访问权限的一组资源。 目录作用域是存储在多个应用程序可理解的目录中的共享作用域。 应用范围是此应用程序仅定义和理解的作用域。|
|directoryScope|[directoryObject](directoryobject.md)|属性引用作为工作分配范围的目录对象。 提供，以便呼叫者可以使用`$expand`与获取角色分配相同的时间获取目录对象。 只读。 |
|appScopeId|String|当分配作用域是特定于应用的应用程序特定作用域的 Id。 工作分配的范围决定了主体已被授予访问权限的一组资源。 目录作用域是存储在多个应用程序可理解的目录中的共享作用域。 对租户范围范围使用 "/"。 应用范围是此应用程序仅定义和理解的作用域。|
|appScope|[appScope](appscope.md)|只读属性，其中包含特定应用程序作用域的详细信息，当分配作用域为应用程序特定时。 包容实体。 |
|resourceScope|String| 应用 unifiedRoleAssignment 的范围。 对于服务范围，这是 "/"。 **请勿使用。此属性将很快被弃用。**|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalId": "String",
  "principal": {"@odata.type": "microsoft.graph.directoryObject"},
  "directoryScopeId": "String",
  "directoryScope": {"@odata.type": "microsoft.graph.directoryObject"},
  "appScopeId": "String",
  "appScope": {"@odata.type": "microsoft.graph.appScope"},
  "resourceScope": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->