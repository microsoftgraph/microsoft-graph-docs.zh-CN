---
title: rbacApplication 资源类型
description: 用于统一角色定义的角色管理容器和用于 RBAC Microsoft 365角色分配。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e6157355fe71d0643c9fff354a4932fc020a9ffd
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454183"
---
# <a name="rbacapplication-resource-type"></a>rbacApplication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于统一角色定义的角色管理容器和用于 RBAC Microsoft 365角色分配。 目前，目录和权利管理是唯一受支持的 RBAC 应用程序。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | 通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignment。 |
| [List roleAssignments](../api/rbacapplication-list-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) 集合 | 获取 unifiedRoleAssignment 对象集合。 通过筛选 roleDefitionId 或 principalId，只能查询特定实例。 |
| [创建 unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。 |
| [List roleDefinitions](../api/rbacapplication-list-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) 集合 | 获取 unifiedRoleDefinition 对象集合。 |
| [roleSchedules](../api/rbacapplication-roleschedules.md) | [unifiedRoleScheduleBase](unifiedroleschedulebase.md) 集合 | 用于检索 unifiedRoleScheduleBase 对象集合的函数。 |
| [roleScheduleInstances](../api/rbacapplication-rolescheduleinstances.md) | [unifiedRoleScheduleInstanceBase](unifiedrolescheduleinstancebase.md) 集合 | 用于检索 unifiedRoleScheduleInstanceBase 对象集合的函数。  |

## <a name="properties"></a>属性

无

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|roleAssignments|[unifiedRoleAssignment](../resources/unifiedroleassignment.md) 集合| 向用户或组授予访问权限的资源。 |
|roleDefinitions|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) 集合| 表示 RBAC 提供程序允许的角色以及分配给角色的权限的资源。 |
|roleAssignmentApprovals|[审批](../resources/approval.md) 集合| 与审批流程角色分配决策。|
|roleAssignmentScheduleInstances|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 集合| 通过 Azure AD 角色分配的活动Privileged Identity Management。  |
|roleAssignmentScheduleRequests|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 集合| 通过 Azure AD 角色分配请求Privileged Identity Management。 |
|roleAssignmentSchedules|[unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md) 集合| 通过 Azure AD 分配计划活动Privileged Identity Management。 |
|roleEligibilityScheduleInstances|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md) 集合| 通过 Azure AD Privileged Identity Management 符合条件的角色分配的实例。 |
|roleEligibilityScheduleRequests|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) 集合| 通过 Azure AD 应用程序请求符合条件的Privileged Identity Management。 |
|roleEligibilitySchedules|[unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md) 集合| 通过 Azure AD 分配计划符合条件的Privileged Identity Management。 |



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


