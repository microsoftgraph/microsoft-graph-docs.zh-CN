---
title: rbacApplicationMultiple 资源类型
description: 角色管理导航属性
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ba6c4973dd79f328c1d04ea26803a6b2aec39c7f
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760916"
---
# <a name="rbacapplicationmultiple-resource-type"></a>rbacApplicationMultiple 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于统一角色定义的角色管理容器，以及支持单个作用域中的多个主体和多个作用域的 Microsoft 365 RBAC 提供程序角色分配。 这不同于 [rbacApplication](rbacapplication.md) 资源类型。 Microsoft Intune 是此类 RBAC 提供程序的一个示例。 Intune 角色分配可以有一个主体数组和一组作用域组。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-post.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignmentMultiple。 |
| [列出 roleAssignmentsMultiple](../api/unifiedroleassignmentmultiple-list.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) 集合 | 获取 unifiedRoleAssignmentMultiple 对象集合。 |
| [创建 unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。 |
| [List roleDefinitions](../api/rbacapplication-list-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) 集合 | 获取 unifiedRoleDefinition 对象集合。 |

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


