---
author: japere
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: ba8ba53c60d37d55cffba7b3f9626832bbf2f1cc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441700"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-pim-v3-api-for-azure-ad-roles-role-management-apis"></a>迁移到面向 Azure AD 角色的 PIM v3 API（角色管理 API）

面向 Azure AD 角色的 PIM API 已于 2021 年 5 月 31 日停用并停止返回数据。 使用本指南将现有 API 迁移到新的 [角色管理 API 以进行特权标识管理](/graph/api/resources/privilegedidentitymanagementv3-overview)。

| Operation | PIM v2 API | 角色管理 API（PIM v3） |
| --------- | ------------ | -------------- |
| 列出角色定义 | [列出 privilegedRoles](/graph/api/privilegedrole-list) | [列出 unifiedRoleDefinitions](/graph/api/rbacapplication-list-roledefinitions) |
| 管理角色设置 | [获取 privilegedRoleSettings](/graph/api/privilegedrolesettings-get)<br/>[更新 privilegedRoleSettings](/graph/api/privilegedrolesettings-update) | [管理策略](/graph/api/policyroot-list-rolemanagementpolicies)
| 创建角色分配请求 | [创建 privilegedRoleAssignmentRequest](/graph/api/privilegedroleassignmentrequest-post) | 使用 [创建 unifiedRoleEligibilityScheduleRequest](/graph/api/rbacapplication-post-roleeligibilityschedulerequests) 创建符合条件的角色分配<br/><br/>使用 [创建 unifiedRoleAssignmentScheduleRequest](/graph/api/rbacapplication-post-roleassignmentschedulerequests) 创建活动角色分配 |
| 列出角色分配 | [列出 privilegedRoleAssignments](/graph/api/privilegedroleassignment-list) | 使用 [列出 unifiedRoleEligibilityScheduleInstances](/graph/api/rbacapplication-list-roleeligibilityscheduleinstances) 获取符合条件的角色分配<br/><br/>使用 [列出 unifiedRoleAssignmentScheduleInstances](/graph/api/rbacapplication-list-roleassignmentscheduleinstances) 获取活动角色分配 |
