---
title: Privileged Identity Management - Azure AD
description: 使用适合于 Azure AD Privileged Identity Management 的 API 管理 Azure Active Directory 角色。
ms.localizationpriority: high
author: carolinetempleton
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 900038e9c68517ac42ade68218b55d7cc52450f9
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688778"
---
# <a name="privileged-identity-management---azure-ad-deprecated"></a>Privileged Identity Management - Azure AD（已弃用）

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1AADRoles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

以下方法由 PIM 针对 Azure AD 角色提供。 此服务构建于 OData 之上。 若要筛选查询中的结果，请在 URL 中使用标准 OData `$filter` 表达式。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列表 privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md) 集合 |获取 privilegedOperationEvent 对象集合。 |
|[获取 privilegedRole](../api/privilegedrole-get.md) |[privilegedRole](privilegedrole.md)| 获取 privilegedRole 对象。|
|[列出 privilegedRole](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md) 集合 |获取 privilegedRole 对象集合。 |
|[列出角色分配](../api/privilegedrole-list-assignments.md) | [privilegedRoleAssignment](privilegedroleassignment.md) 集合 |获取特定角色的 privilegedRoleAssignment 集合。 每个 privilegedRoleAssignment 表示为用户分配的角色。|
|[selfActivate](../api/privilegedrole-selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |激活分配给请求者的角色。|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |停用分配给请求者的角色。|
|[创建 privilegedRoleAssignment](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| 通过发布到 privilegedRoleAssignments 集合新建 privilegedRoleAssignment（角色分配）。|
|[列出 privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) 集合 |获取 privilegedRoleAssignment 对象集合。 该集合包含组织的所有角色分配。 每个 privilegedRoleAssignment 表示为用户分配的角色。 |
|[获取 privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|获取具有指定分配 id 的 privilegedRoleAssignment 对象。 |
|[Delete privilegedRoleAssignment](../api/privilegedroleassignment-delete.md) | 无。 |删除 privilegedRoleAssignment 对象。 |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |将角色分配标记为永久。 |
|[makeEligible](../api/privilegedroleassignment-makeeligible.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |使角色分配符合资格。 |
|[My](../api/privilegedroleassignment-my.md) | [privilegedRoleAssignment](privilegedroleassignment.md) 集合|获取请求者的角色分配。 |
|[获取 privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|检索 privilegedRoleSettings 对象的属性。 |
|[获取 privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|检索 privilegedRoleSummary 对象。 |
|[获取 privilegedApproval](../api/privilegedapproval-get.md) |[privilegedApproval](privilegedapproval.md)| 获取 privilegedApproval 对象。|
|[列出 privilegedApproval](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md) 集合 |Get privilegedApproval 对象集合。 |
|[创建 privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |创建 privilegedApproval 对象。 |
|[更新 privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |更新 privilegedApproval 对象。 |
|[myrequests](../api/privilegedapproval-myrequests.md) | [privilegedApproval](privilegedapproval.md) 集合|获取请求者的审批请求。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
