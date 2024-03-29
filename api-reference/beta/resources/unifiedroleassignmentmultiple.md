---
title: unifiedRoleAssignmentMultiple 资源类型
description: 分配给主体数组的角色定义 (通常是用户) 一组作用域。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4dc43e36ce1f224a920f99d02210268d68b42d40
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764029"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a>unifiedRoleAssignmentMultiple 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

unifiedRoleAssignmentMultiple 用于授予对资源的访问权限，作为 RBAC 角色Microsoft 365的一[部分](rolemanagement.md)。 它表示分配给主体数组的角色定义 (通常是用户) 一组作用域。 

可以创建具有角色分配和多个作用域的组。

你必须提供 **directoryScopeIds** **或 appScopeIds**。

目前支持以下 RBAC 提供程序：
- 云电脑 
- Microsoft Intune

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [List roleAssignments](../api/rbacapplicationmultiple-list-roleassignments.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) 集合 | 读取 unifiedRoleAssignmentMultiple 对象及其属性的列表。 |
| [创建 unifiedRoleAssignmentMultiple](../api/rbacapplicationmultiple-post-roleassignments.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignmentMultiple。 |
| [获取 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 读取 unifiedRoleAssignmentMultiple 对象的属性和关系。 |
| [更新 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 更新现有的 unifiedRoleAssignmentMultiple 对象。 |
| [删除 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md) | 无 | 删除 unifiedRoleAssignmentMultiple 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| appScopeIds | String collection | 当分配范围特定于应用时，特定于应用的范围的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 用于 `/` 租户范围范围。 应用程序作用域是仅由此应用程序定义和理解的范围。 |
| 说明 | String | 角色分配。 |
| directoryScopeIds | String collection | 表示工作分配范围的目录对象的 ID。 工作分配的范围决定了已授予主体访问权限的资源集。 目录作用域是存储在目录中的多个应用程序可以理解的共享范围。 应用程序作用域是仅由此应用程序定义和理解的范围。 |
| displayName | String | 域名角色分配。 必需。 |
| id | String | unifiedRoleAssignmentMultiple 的唯一标识符。 键，不可为 null，只读。 |
| roleDefinitionId | String | 分配所针对的 unifiedRoleDefinition 的标识符。 |
| principalIds | String collection | 分配授予的主体的标识符。  仅 `$filter` (`any` 运算符) 。 |


## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| appScopes | [appScope](appscope.md) 集合 |当分配范围特定于应用时，具有特定于应用的范围的详细信息的只读集合。 包含实体。 只读。  |
| directoryScopes | [directoryObject](directoryobject.md) 集合 | 引用作为分配范围的目录对象的只读集合。 提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。 只读。  支持 `$expand`。|
| principals| [directoryObject](directoryobject.md) 集合 | 引用分配的主体的只读集合。 提供此权限，以便调用方可以使用 与获取权限 `$expand` 角色分配。 只读。  支持 `$expand`。|
| roleDefinition | [unifiedRoleDefinition](unifiedroledefinition.md) |指定分配用于的 roleDefinition。 提供，以便调用方可以在获取角色定义的同时使用 `$expand` 角色分配。  支持 `$filter` (`eq` **id** **、isBuiltIn** 和 displayName 上的 **displayName** 和) `startsWith`  `$expand` 运算符。 |


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


