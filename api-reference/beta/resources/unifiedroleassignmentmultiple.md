---
title: unifiedRoleAssignmentMultiple 资源类型
description: 角色分配是角色定义与特定作用域的主体之间的链接，用于授予访问权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f612fea9ce7aa54cce505a4f2d77370f45947c44
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442689"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>unifiedRoleAssignmentMultiple 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

unifiedRoleAssignmentMultiple 用于授予对资源的访问权限。 它表示分配给主体数组的角色定义 (通常是用户) 一组主体。 Microsoft Intune 就是此类 RBAC 提供程序的一个示例。 在 Microsoft Intune 中，你可以创建一角色分配多个主体和多个作用域的 Microsoft Intune。

需要 **提供 directoryScopeIds** **或 appScopeIds。**

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
| id | String | unifiedRoleAssignmentMultiple 的唯一标识符。 键，不可为 null，只读。 |
| displayName | String | 名称角色分配。 必需。 |
| description | String | 说明角色分配。 |
| roleDefinitionId | String | 工作分配的 unifiedRoleDefinition 的 ID。 |
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |指示工作分配所针对的 roleDefinition 的属性。 已提供，以便调用方可以在获取角色定义的同时获取 `$expand` 角色分配。 只读。  |
| principalIds | 字符串集合 | 分配所授予的主体的 Objectid。 |
| 主体| [directoryObject](directoryobject.md) 集合 | 引用分配的主体的只读集合。 提供，以便调用方可以在获取主服务器时同时 `$expand` 角色分配。 只读。 |
| directoryScopeIds | 字符串集合 | 表示工作分配范围的目录对象的 ID。 工作分配的范围决定了主体已被授予访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 应用范围是仅此应用程序定义和了解的范围。 |
| directoryScopes | [directoryObject](directoryobject.md) 集合 | 引用作为分配范围的目录对象的只读集合。 提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。 只读。 |
| appScopeIds | 字符串集合 | 当分配范围特定于应用时，应用特定范围的 ID。 工作分配的范围决定了主体已被授予访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 对租户范围使用"/"。 应用范围是仅此应用程序定义和了解的范围。 |
| appScopes | [appScope](appscope.md) 集合 |当分配范围特定于应用时，具有特定于应用范围的详细信息的只读集合。 包含实体。 只读。  |

## <a name="relationships"></a>关系

无

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


