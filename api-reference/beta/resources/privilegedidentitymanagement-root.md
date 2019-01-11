---
title: Azure AD 权限身份管理
description: 下面是由特权身份管理服务所提供的方法的列表。
localization_priority: Priority
ms.openlocfilehash: c1108711c96dd253f784a418a396ca30507c5f7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884061"
---
# <a name="azure-ad-privileged-identity-management"></a>Azure AD 权限身份管理

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

下面是由[特权身份管理](https://azure.microsoft.com/en-us/documentation/articles/active-directory-privileged-identity-management-configure/)服务所提供的方法的列表。

该服务构建于 OData。 若要筛选查询的结果，请使用标准 OData ``$filter`` Uri 中的表达式。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md)集合 |获取 privilegedOperationEvent 对象集合。 |
|[获取 privilegedRole](../api/privilegedrole-get.md) |[privilegedRole](privilegedrole.md)| 获取 privilegedRole 对象。|
|[列表 privilegedRole](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md)集合 |获取 privilegedRole 对象集合。 |
|[列表角色分配](../api/privilegedrole-list-assignments.md) | [privilegedRoleAssignment](privilegedroleassignment.md)集合 |获取特定的角色 privilegedRoleAssignment 集合。 每个 privilegedRoleAssignment 代表角色分配给用户。|
|[selfActivate](../api/privilegedrole-selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |激活分配给请求者角色。|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |停用的角色分配给请求者。|
|[创建 privilegedRoleAssignment](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| 通过发布到 privilegedRoleAssignments 集合中创建新 privilegedRoleAssignment （工作分配角色）。|
|[列表 privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md)集合 |获取 privilegedRoleAssignment 对象集合。 集合中包含组织的所有角色的分配。 每个 privilegedRoleAssignment 代表角色分配给用户。 |
|[获取 privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|获取具有指定的工作分配 id privilegedRoleAssignment 对象。 |
|[删除 privilegedRoleAssignment](../api/privilegedroleassignment-delete.md) | 无。 |删除 privilegedRoleAssignment 对象。 |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |请为永久的角色分配。 |
|[makeEligible](../api/privilegedroleassignment-makeeligible.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |请作为合格的角色分配。 |
|[我](../api/privilegedroleassignment-my.md) | [privilegedRoleAssignment](privilegedroleassignment.md)集合|获取请求者的角色分配。 |
|[获取 privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|检索 privilegedRoleSettings 对象的属性。 |
|[获取 privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|检索 privilegedRoleSummary 对象。 |
|[获取 privilegedApproval](../api/privilegedapproval-get.md) |[privilegedApproval](privilegedapproval.md)| 获取 privilegedApproval 对象。|
|[列表 privilegedApproval](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md)集合 |获取 privilegedApproval 对象集合。 |
|[创建 privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |创建 privilegedApproval 对象。 |
|[更新 privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |更新 privilegedApproval 对象。 |
|[myrequests](../api/privilegedapproval-myrequests.md) | [privilegedApproval](privilegedapproval.md)集合|获取请求者的审批请求。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
