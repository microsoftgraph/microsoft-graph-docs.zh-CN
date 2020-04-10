---
title: unifiedRoleAssignmentMultiple 资源类型
description: 角色分配是角色定义和特定作用域的主体之间的链接，目的是为了授予访问权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 20e0d7a213ea6e46db9cf9774c46bda0070ecd27
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218028"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>unifiedRoleAssignmentMultiple 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

UnifiedRoleAssignmentMultiple 用于授予对资源的访问权限。 它表示分配给范围数组的主体（通常为用户）数组的角色定义。 此类 RBAC 提供程序的一个示例是 Microsoft Intune。 在 Microsoft Intune 中，可以创建具有多个主体和多个作用域的角色分配。

提供 " **directoryScopeIds** " 或 " **appScopeIds** " 是必需的。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 读取 unifiedRoleAssignmentMultiple 对象的属性和关系。 |
| [创建 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignmentMultiple。 |
| [更新 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 更新现有的 unifiedRoleAssignmentMultiple 对象。 |
| [删除 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | 无 | 删除 unifiedRoleAssignmentMultiple 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| id | 字符串 | UnifiedRoleAssignmentMultiple 的唯一标识符。 键，不可为 null，只读。 |
| displayName | String | 角色分配的名称。 |
| 说明 | String | 角色分配的说明。 |
| roleDefinitionId | 字符串 | 工作分配所针对的 unifiedRoleDefinition 的 ID。 只读。 |
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |指示工作分配所针对的 roleDefinition 的属性。 提供，以便呼叫者可以在获取角色分配`$expand`的同时使用该角色定义。 |
| principalIds | String collection | 向其授予分配的主体的 Objectids。 |
| 原理| [directoryObject](directoryobject.md) 集合 | 引用所分配的主体的只读集合。 提供，以便呼叫者可以在获取角色`$expand`分配的同时使用这些承担者。 只读。 |
| directoryScopeIds | String collection | 表示工作分配范围的目录对象的 id。 工作分配的范围决定了主体已被授予访问权限的资源集。 目录作用域是存储在多个应用程序可理解的目录中的共享作用域。 应用范围是此应用程序仅定义和理解的作用域。 |
| directoryScopes | [directoryObject](directoryobject.md) 集合 | 只读集合，引用属于分配范围的目录对象。 提供，以便呼叫者可以使用`$expand`与获取角色分配相同的时间获取目录对象。 只读。 |
| appScopeIds | String collection | 当分配作用域是特定于应用的应用程序特定作用域的 id。 工作分配的范围决定了主体已被授予访问权限的一组资源。 目录作用域是存储在多个应用程序可理解的目录中的共享作用域。 对租户范围范围使用 "/"。 应用范围是此应用程序仅定义和理解的作用域。 |
| appScopes | [appScope](appscope.md)集合 |只读集合，其中包含应用程序特定作用域的详细信息，当分配作用域为应用程序特定时。 包容实体。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalIds": ["string"],
  "principals": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "directoryScopeIds": ["string"],
  "directoryScopes": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "appScopeIds": ["string"],
  "appScopes": [{"@odata.type": "microsoft.graph.appScope"}],
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignmentMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->