---
title: unifiedRoleAssignment 资源类型
description: 角色分配是角色定义和特定作用域的主体之间的链接，目的是为了授予访问权限。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c51c3cd7c706cf154db8c1de21c04aaa098c3efb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519615"
---
# <a name="unifiedroleassignment-resource-type"></a>unifiedRoleAssignment 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

UnifiedRoleAssignment 用于授予对资源的访问权限。 它表示分配给特定范围内的主体（通常为用户）的角色定义。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 unifiedRoleAssignment](../api/unifiedroleassignment-get.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | 读取 unifiedRoleAssignment 对象的属性和关系。 |
| [创建 unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | 通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignment。 |
| [删除](../api/unifiedroleassignment-delete.md) | 无 | 删除 unifiedRoleAssignment 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| UnifiedRoleAssignment 的唯一标识符。 键，不可为 null，只读。 |
|principalId|String| 向其授予分配的主体的 Objectid。 |
|resourceScope|String| 应用 unifiedRoleAssignment 的范围。 对于服务范围，这是 "/"。 |
|roleDefinitionId|String| 工作分配的 unifiedRoleDefinition。 只读。 |

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
  "principalId": "String",
  "resourceScope": "String",
  "roleDefinitionId": "String"
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
