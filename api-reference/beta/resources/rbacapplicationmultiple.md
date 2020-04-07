---
title: rbacApplicationMultiple 资源类型
description: 角色管理导航属性
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c89b9e12121fc5c3183629b6349d04d5dd434cab
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160335"
---
# <a name="rbacapplicationmultiple-resource-type"></a>rbacApplicationMultiple 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于在单个角色分配中支持多个主体和多个作用域的 Microsoft 365 RBAC 提供程序的统一角色定义和角色分配的角色管理容器。 这不同于[rbacApplication](rbacapplication.md)资源类型。 Microsoft Intune 是此类 RBAC 提供程序的一个示例。 Intune 中的角色分配可以具有主体阵列和作用域组的阵列。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignmentMultiple。 |
| [列出 roleAssignmentsMultiple](../api/unifiedroleassignmentmultiple-list.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md)集合 | 获取 unifiedRoleAssignmentMultiple 对象集合。 通过在 unifiedRoleDefitionId 或 principalId 上进行筛选，只能查询特定的实例。 |
| [创建 unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。 |
| [List roleDefinitions](../api/rbacapplication-list-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md)集合 | 获取 unifiedRoleDefinition 对象集合。 |

## <a name="properties"></a>属性

无

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

无

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->