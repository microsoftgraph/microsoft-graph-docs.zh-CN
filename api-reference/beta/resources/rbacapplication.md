---
title: rbacApplication 资源类型
description: 用于 Microsoft 365 RBAC 提供程序的统一角色定义和角色分配的角色管理容器。
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 74b6fe87456108ba66bf4db4363434cc45133ce9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336765"
---
# <a name="rbacapplication-resource-type"></a>rbacApplication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于 Microsoft 365 RBAC 提供程序的统一角色定义和角色分配的角色管理容器。 目前，目录和权利管理是唯一受支持的 RBAC 应用程序。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [创建 unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | 通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignment。 |
| [List roleAssignments](../api/rbacapplication-list-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) 集合 | 获取 unifiedRoleAssignment 对象集合。 通过筛选 roleDefitionId 或 principalId，只能查询特定实例。 |
| [列出 transitiveRoleAssignments](../api/rbacapplication-list-transitiveroleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) 集合 | 获取分配给特定主体的直接且可传递的 unifiedRoleAssignments。 指定 principalId 是必需的。 |
| [创建 unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | 通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。 |
| [List roleDefinitions](../api/rbacapplication-list-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) 集合 | 获取 unifiedRoleDefinition 对象集合。 |
| [roleSchedules](../api/rbacapplication-roleschedules.md) | [unifiedRoleScheduleBase](unifiedroleschedulebase.md) 集合 | 用于检索 unifiedRoleScheduleBase 对象集合的函数。 |
| [roleScheduleInstances](../api/rbacapplication-rolescheduleinstances.md) | [unifiedRoleScheduleInstanceBase](unifiedrolescheduleinstancebase.md) 集合 | 用于检索 unifiedRoleScheduleInstanceBase 对象集合的函数。  |

## <a name="properties"></a>属性

无

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|resourceNamespaces|[unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md) 集合|表示相关操作集合的资源。|
|roleAssignments|[unifiedRoleAssignment](../resources/unifiedroleassignment.md) 集合| 向用户或组授予访问权限的资源。 |
|roleDefinitions|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) 集合| 表示 RBAC 提供程序允许的角色以及分配给角色的权限的资源。 |
|roleAssignmentApprovals|[审批](../resources/approval.md) 集合| 与审批流程角色分配决策。|
|roleAssignmentScheduleInstances|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) 集合| 通过 Azure AD Privileged Identity Management 进行活动角色分配的实例。  |
|roleAssignmentScheduleRequests|[unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md) 集合| 通过 Azure AD Privileged Identity Management 请求活动角色分配。 |
|roleAssignmentSchedules|[unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md) 集合| 通过 Azure AD Privileged Identity Management 安排活动角色分配。 |
|roleEligibilityScheduleInstances|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md) 集合| 通过 Azure AD Privileged Identity Management 的合格角色分配的实例。 |
|roleEligibilityScheduleRequests|[unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md) 集合| 通过 Azure AD Privileged Identity Management 请求符合条件的角色分配。 |
|roleEligibilitySchedules|[unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md) 集合| 通过 Azure AD Privileged Identity Management 计划符合条件的角色分配。 |
|transitiveRoleAssignments|[unifiedRoleAssignment](../resources/unifiedroleassignment.md) 集合| 向可传递的用户或组授予访问权限的资源。 |


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


