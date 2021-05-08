---
title: unifiedRoleAssignmentMultiple 资源类型
description: 分配给主体数组的角色定义 (通常是用户) 一组主体。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b6f345dbf4947212f22a5386fded551d62b0e24d
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241056"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>unifiedRoleAssignmentMultiple 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

unifiedRoleAssignmentMultiple 用于授予对资源的访问权限。 它表示分配给主体数组的角色定义 (通常是用户通过) 组进行分配。 此类 RBAC 提供程序的一个示例是Microsoft Intune。 在Microsoft Intune中，可以创建具有角色分配和多个作用域的组。

需要 **提供 directoryScopeIds** 或 **appScopeIds。**

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-list.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 读取 unifiedRoleAssignmentMultiple 对象及其属性的列表。 |
| [获取 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 读取 unifiedRoleAssignmentMultiple 对象的属性和关系。 |
| [创建 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignmentMultiple。 |
| [更新 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 更新现有的 unifiedRoleAssignmentMultiple 对象。 |
| [删除 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | 无 | 删除 unifiedRoleAssignmentMultiple 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| id | 字符串 | unifiedRoleAssignmentMultiple 的唯一标识符。 键，不可为 null，只读。 |
| displayName | 字符串 | 域名角色分配。 必需。 |
| description | 字符串 | 项目说明角色分配。 |
| roleDefinitionId | 字符串 | 分配所针对的 unifiedRoleDefinition 的标识符。 |
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |指示分配所针对的 roleDefinition 的属性。 提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。 只读。 支持 `$filter` (`eq` **id** **、isBuiltIn** 和 **displayName** 上的 `startsWith` **displayName** 和) `$expand` 运算符。  |
| principalIds | String collection | 分配授予的主体的标识符。  仅 `$filter` (`any` 运算符) 。 |
| directoryScopeIds | String collection | 表示工作分配范围的目录对象的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 应用程序作用域是仅由此应用程序定义和理解的范围。 |
| appScopeIds | String collection | 当分配范围特定于应用时，特定于应用的范围的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 应用程序作用域是仅由此应用程序定义和理解的范围。 |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| appScopes | [appScope](appscope.md) 集合 |当分配范围特定于应用时，具有特定于应用的范围的详细信息的只读集合。 包含实体。 只读。  |
| directoryScopes | [directoryObject](directoryobject.md) collection | 引用作为分配范围的目录对象的只读集合。 提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。 只读。  支持 `$expand`。|
| principals| [directoryObject](directoryobject.md) collection | 引用分配的主体的只读集合。 提供此权限，以便调用方可以使用 与获取 角色分配 `$expand` 同时使用。 只读。  支持 `$expand`。|
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|分配用于的 roleDefinition。 提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。 **roleDefinition.id** 自动展开。 支持 `$expand`。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
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


