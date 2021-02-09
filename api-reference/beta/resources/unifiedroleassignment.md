---
title: unifiedRoleAssignment 资源类型
description: 一角色分配是角色定义与特定作用域的主体之间的链接，用于授予访问权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4dc0ec6bb692c88d2b01a440bae1d7789bd042a5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159022"
---
# <a name="unifiedroleassignment-resource-type"></a>unifiedRoleAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

unifiedRoleAssignment 用于授予对资源的访问权限。 它表示分配给主体的角色定义 (通常是特定) 用户的角色定义。

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
|id|String| unifiedRoleAssignment 的唯一标识符。 键，不可为 null，只读。 |
|roleDefinitionId|String| 分配所针对的 unifiedRoleDefinition 的 ID。 只读。 |
|roleDefinition|[unifiedRoleDefinition](unifiedroledefinition.md)|指示工作分配所针对的角色定义的属性。 提供，以便调用方可以在获取角色定义的同时获取 `$expand` 角色分配。 roleDefinition.Id自动展开
|principalId|String| 分配授予的主体的 Objectid。 |
|principal|[directoryObject](directoryobject.md)| 引用分配的主体的属性。 提供此权限，以便调用方可以同时使用主体获取 `$expand` 角色分配。 只读。 |
|directoryScopeId|String|表示工作分配范围的目录对象的 ID。 工作分配的范围决定了主体已被授予访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 应用范围是仅由此应用程序定义和理解的范围。|
|directoryScope|[directoryObject](directoryobject.md)|引用作为分配范围的目录对象的属性。 提供，以便调用方可以在获取目录对象的同时获取 `$expand` 角色分配。 只读。 |
|appScopeId|String|当分配范围特定于应用时，应用特定范围的 ID。 工作分配的范围决定了主体已被授予访问权限的资源集。 目录范围是存储在目录中的多个应用程序可以理解的共享范围。 对租户范围范围使用"/"。 应用范围是仅由此应用程序定义和理解的范围。|
|appScope|[appScope](appscope.md)|当分配范围特定于应用时，具有特定于应用范围的详细信息的只读属性。 包含实体。 |
|resourceScope|String| unifiedRoleAssignment 适用的范围。 对于服务范围，这是"/"。 **请勿使用。此属性将很快弃用。**|

## <a name="relationships"></a>关系

无

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

