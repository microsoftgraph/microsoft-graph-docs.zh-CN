---
title: rbacApplicationMultiple 资源类型
description: 角色管理导航属性
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: df5c5cd1421d4601357ef2d48c00b693e6c5e324
ms.sourcegitcommit: 30903b12daf4cf2841524c57743889e23d11f85a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2021
ms.locfileid: "53533862"
---
# <a name="rbacapplicationmultiple-resource-type"></a>rbacApplicationMultiple 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于统一角色定义和角色分配的角色管理容器Microsoft 365一个角色集中支持多个主体和多个作用域的 RBAC 角色分配。 

这不同于 [rbacApplication](rbacapplication.md) 资源类型。 

云电脑Microsoft Intune是此类 RBAC 提供程序的示例。 这些角色分配中的服务器可以具有一组主体和一组范围组。

对于角色定义，云电脑提供商当前支持 [列表](../api/rbacapplication-list-roledefinitions.md) 操作，但支持 [创建](../api/rbacapplication-post-roledefinitions.md)。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。 |
| [List roleDefinitions](../api/rbacapplication-list-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) 集合 | 获取 unifiedRoleDefinition 对象集合。 |
| [创建 unifiedRoleAssignmentMultiple](../api/rbacapplicationmultiple-post-roleassignments.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) | 通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignmentMultiple。 |
| [List roleAssignments](../api/rbacapplicationmultiple-list-roleassignments.md) | [unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) 集合 | 获取 unifiedRoleAssignmentMultiple 对象集合。 |

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


