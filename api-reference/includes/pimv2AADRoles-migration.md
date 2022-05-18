---
author: japere
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: f956f82fbfb6488f23f7ae155d49c1344ec890e2
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461281"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-pim-v3-api-for-azure-ad-roles-role-management-apis"></a>迁移到面向 Azure AD 角色的 PIM v3 API（角色管理 API）

面向 Azure AD 角色的 PIM API 已于 2021 年 5 月 31 日停用并停止返回数据。 使用本指南将现有 API 迁移到新的 [角色管理](/graph/api/resources/privilegedidentitymanagementv3-overview.md?view=graph-rest-beta&preserve-view=true) API。

| Operation | PIM v2 API | 角色管理 API（PIM v3） |
| --------- | ------------ | -------------- |
| 列出角色定义 | [列出 privilegedRoles](/graph/api/privilegedrole-list) | [列出 unifiedRoleDefinitions](/graph/api/rbacapplication-list-roledefinitions) |
| 管理角色设置 | [获取 privilegedRoleSettings](/graph/api/privilegedrolesettings-get)<br/>[更新 privilegedRoleSettings](/graph/api/privilegedrolesettings-update) | [管理策略](/graph/api/policyroot-list-rolemanagementpolicies)
| 创建角色分配请求 | [创建 privilegedRoleAssignmentRequest](/graph/api/privilegedroleassignmentrequest-post) | 使用 [创建 unifiedRoleEligibilityScheduleRequest](/graph/api/rbacapplication-post-roleeligibilityschedulerequests) 创建符合条件的角色分配<br/><br/>使用 [创建 unifiedRoleAssignmentScheduleRequest](/graph/api/rbacapplication-post-roleassignmentschedulerequests) 创建活动角色分配 |
| 列出角色分配 | [列出 privilegedRoleAssignments](/graph/api/privilegedroleassignment-list) | 使用 [列出 unifiedRoleEligibilityScheduleInstances](/graph/api/rbacapplication-list-roleeligibilityscheduleinstances) 获取符合条件的角色分配<br/><br/>使用 [列出 unifiedRoleAssignmentScheduleInstances](/graph/api/rbacapplication-list-roleassignmentscheduleinstances) 获取活动角色分配 |