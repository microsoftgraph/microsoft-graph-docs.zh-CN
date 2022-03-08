---
title: unifiedRoleAssignment 资源类型
description: 一角色分配是角色定义与特定作用域的主体之间的链接，用于授予访问权限。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b7500c3d332b26a3078ed16f3e589e5125deb9f8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335974"
---
# <a name="unifiedroleassignment-resource-type"></a>unifiedRoleAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

unifiedRoleAssignment 用于授予对资源的访问权限。 它表示分配给主体的角色定义 (通常是特定) 用户的角色定义。

需要提供 directoryScopeId 或 appScopeId。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 unifiedRoleAssignment](../api/rbacapplication-list-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | 读取 unifiedRoleAssignment 对象及其属性的列表。 |
| [列出 transitiveRoleAssignments](../api/rbacapplication-list-transitiveroleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) 集合 | 获取分配给特定主体的直接且可传递的 unifiedRoleAssignments。 指定 principalId 是必需的。 |
| [获取 unifiedRoleAssignment](../api/unifiedroleassignment-get.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | 读取 unifiedRoleAssignment 对象的属性和关系。 |
| [创建 unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | 通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignment。 |
| [删除 unifiedRoleAssignment](../api/unifiedroleassignment-delete.md) | 无 | 删除 unifiedRoleAssignment 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| unifiedRoleAssignment 的唯一标识符。 键，不可为 null，只读。 |
|roleDefinitionId|字符串| 分配所针对的 unifiedRoleDefinition 的标识符。 只读。 仅 `$filter` (`eq` 运算符) 。 |
|principalId|字符串| 分配授予的主体的标识符。 仅 `$filter` (`eq` 运算符) 。 |
|directoryScopeId|String|表示工作分配范围的目录对象的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 应用程序作用域是仅由此应用程序定义和理解的范围。|
|appScopeId|String|当分配范围特定于应用时，特定于应用的范围的标识符。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 应用程序作用域是仅由此应用程序定义和理解的范围。  对于权利管理提供程序，使用应用程序范围指定目录，例如 `/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997`。|
|resourceScope|字符串| unifiedRoleAssignment 适用的范围。 这 `/` 适用于服务范围。 **请勿使用。此属性将很快弃用。**|

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|appScope|[appScope](appscope.md)|当分配范围特定于应用时，特定于应用的范围的详细信息。 包含实体。 |
|directoryScope|[directoryObject](directoryobject.md)|分配范围的目录对象。 提供，以便调用方可以在获取目录对象 `$expand` 的同时获取角色分配。 只读。 支持 `$expand`。 |
|principal|[directoryObject](directoryobject.md)| 分配的主体。 提供此权限，以便调用方 `$expand` 可以使用 与获取权限相同的角色分配。 只读。 支持 `$expand`。 |
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|分配用于的 roleDefinition。 提供，以便调用方可以在 `$expand` 获取角色定义的同时使用 角色分配。 **roleDefinition.id** 自动展开。 支持 `$expand`。 |



## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
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
