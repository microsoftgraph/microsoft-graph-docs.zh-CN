---
author: carolinetempleton
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: 380107ef1adb54df7452a8baa157e446cf44dd35
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "64477837"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-pim-v3-api-for-azure-ad-roles-role-management-apis"></a>迁移到面向 Azure AD 角色的 PIM v3 API（角色管理 API）

面向 Azure AD 角色的 PIM API 已于 2021 年 5 月 31 日停用并停止返回数据。 使用本指南将现有 API 迁移到新的 [角色管理](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) API。

| Operation | PIM v2 API | 角色管理 API（PIM v3） |
| --------- | ------------ | -------------- |
| 列出角色定义 | [列出 privilegedRoles](/graph/api/privilegedrole-list) | [列出 unifiedRoleDefinitions](/graph/api/rbacapplication-list-roledefinitions) |
| 管理角色设置 | [获取 privilegedRoleSettings](/graph/api/privilegedrolesettings-get)<br/>[更新 privilegedRoleSettings](/graph/api/privilegedrolesettings-update) | [管理策略](/graph/api/unifiedrolemanagementpolicy-list)
| 创建角色分配请求 | [创建 privilegedRoleAssignmentRequest](/graph/api/privilegedroleassignmentrequest-post) | 使用 [创建 unifiedRoleEligibilityScheduleRequest](/graph/api/unifiedroleeligibilityschedulerequest-post-unifiedroleeligibilityschedulerequests) 创建符合条件的角色分配<br/><br/>使用 [创建 unifiedRoleAssignmentScheduleRequest](/graph/api/unifiedroleassignmentschedulerequest-post-unifiedroleassignmentschedulerequests) 创建活动角色分配 |
| 列出角色分配 | [列出 privilegedRoleAssignments](/graph/api/privilegedroleassignment-list) | 使用 [列出 unifiedRoleEligibilityScheduleInstances](/graph/api/unifiedroleeligibilityscheduleinstance-list) 获取符合条件的角色分配<br/><br/>使用 [列出 unifiedRoleAssignmentScheduleInstances](/graph/api/unifiedroleassignmentscheduleinstance-list) 获取活动角色分配 |