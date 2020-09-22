---
title: rbacApplication 资源类型
description: 角色管理导航属性
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e7145509745bdb696ebe3342035096af27d89b38
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993047"
---
# <a name="rbacapplication-resource-type"></a>rbacApplication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

适用于 Microsoft 365 RBAC 提供程序的统一角色定义和角色分配的角色管理容器。 当前 "目录" 是唯一受支持的 RBAC 应用程序。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | 通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignment。 |
| [List roleAssignments](../api/rbacapplication-list-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) 集合 | 获取 unifiedRoleAssignment 对象集合。 通过在 roleDefitionId 或 principalId 上进行筛选，只能查询特定的实例。 |
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
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


