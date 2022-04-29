---
title: 通过特权标识管理 (PIM) API 进行角色管理概述
description: Privileged Identity Management (PIM) 是Azure AD标识治理的一项功能，可用于管理、控制和监视对组织中重要资源的访问。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6293582e47eccc81ee3ac7ecbc47e9e8e6f38082
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134056"
---
# <a name="overview-of-role-management-through-the-privileged-identity-management-pim-api"></a>通过特权标识管理 (PIM) API 进行角色管理概述

命名空间：microsoft.graph

Privileged Identity Management (PIM) 是[Azure AD标识治理](/azure/active-directory/governance/identity-governance-overview)的一项功能，可用于管理、控制和监视对组织中重要资源的访问。 此访问通过特权角色和基于角色的访问控制 (RBAC) 启用，并且可以授予用户、组或服务主体。 资源可以位于 Azure AD、Azure 和其他 Microsoft Online Services（如 Microsoft 365 或 Microsoft Intune）中。

用于角色管理的 Microsoft Graph PIM API 允许你管理特权访问并限制过度访问。 本文介绍 Microsoft Graph 中 PIM API 的治理功能。

> [!NOTE]
> 若要管理 Azure 资源角色，请使用[适用于 PIM 的 Azure 资源管理器 (ARM) API](/rest/api/authorization/privileged-role-eligibility-rest-sample)。

## <a name="pim-api-for-managing-role-assignments"></a>用于管理角色分配的 PIM API

PIM 允许通过创建永久性分配或临时分配来管理活动角色分配。 使用 [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) 资源类型及其相关方法来管理角色分配。

下表列出了使用 PIM 管理角色分配和要调用的 API 的方案：

|应用场景  |API  |
|---------|---------|
|管理员创建并分配给主体永久角色分配  <br/> 管理员向主体分配临时角色   |   [创建 roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|管理员续订、更新、扩展或删除角色分配     |   [创建 roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|管理员查询所有角色分配及其详细信息     |   [列出 roleAssignmentScheduleRequests](../api/rbacapplication-list-roleassignmentschedulerequests.md)      |
|管理员查询角色分配及其详细信息     |   [获取 unifiedRoleAssignmentScheduleRequest](../api/unifiedroleassignmentschedulerequest-get.md)      |
|主体查询其角色分配和详细信息     |  [unifiedRoleAssignmentScheduleRequest：filterByCurrentUser](../api/unifiedroleassignmentschedulerequest-filterbycurrentuser.md)       |
|主体对其 *符合条件* 的角色分配执行实时和限时激活     |   [创建 roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|主体取消他们创建的角色分配请求     |   [unifiedRoleAssignmentScheduleRequest：cancel](../api/unifiedroleassignmentschedulerequest-cancel.md)      |
|激活其符合条件的角色分配的主体在不再需要访问权限时停用它     |   [创建 roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |
|主体停用、扩展或续订其角色分配。     |   [创建 roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md)      |

## <a name="pim-api-for-managing-role-eligibilities"></a>用于管理角色可视化的 PIM API

主体可能不需要永久角色分配，因为它们可能不需要一直通过特权角色授予的特权。 在这种情况下，PIM 还允许你创建角色可变性并将其分配给主体。 使用角色可选性，主体在需要执行特权任务时激活角色。 激活始终为最长 8 小时的时间限制。 角色资格也可以是永久资格或临时资格。

使用  [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) 资源类型及其相关方法来管理角色可变性。

下表列出了使用 PIM 管理角色可取性和要调用的 API 的方案：

|应用场景  |API  |
|---------|---------|
|管理员创建并分配给主体一个符合条件的角色  <br/> 管理员将临时角色资格分配给主体   |   [创建 roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md)      |
|管理员续订、更新、扩展或删除角色可伸缩性     |   [创建 roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md)      |
|管理员查询所有角色可选性及其详细信息     |   [列出 roleEligibilityScheduleRequests](../api/rbacapplication-list-roleeligibilityschedulerequests.md)      |
|管理员查询角色资格及其详细信息     |   [获取 unifiedRoleEligibilityScheduleRequest](../api/unifiedroleeligibilityschedulerequest-get.md)      |
|管理员取消他们创建的角色资格请求     |   [unifiedRoleEligibilityScheduleRequest： cancel](../api/unifiedroleeligibilityschedulerequest-cancel.md)      |
|主体查询其角色质询和详细信息     |  [unifiedRoleEligibilityScheduleRequest： filterByCurrentUser](../api/unifiedroleeligibilityschedulerequest-filterbycurrentuser.md)       |
|主体停用、扩展或续订其角色资格。     |   [创建 roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md)      |


## <a name="role-settings-and-pim"></a>角色设置和 PIM

每个Azure AD角色定义设置或规则。 此类设置包括激活符合条件的角色是否需要多重身份验证 (MFA) 、理由或审批。 或者，是否可以为角色的主体创建永久性分配或可取性。 这些特定于角色的设置将确定通过 PIM 创建或管理角色分配和可实现的设置。 在 Microsoft Graph中，这些角色设置通过 [unifiedRoleManagementPolicy 资源类型](unifiedrolemanagementpolicy.md)和相关方法公开。

例如，假定默认情况下，角色不允许永久活动分配，并且为活动分配定义最多 15 天。 尝试在没有过期日期的情况下创建 [unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) 对象将返回 `400 Bad Request` 违反过期规则的响应代码。

使用 [unifiedRoleManagementPolicyAssignment](unifiedrolemanagementpolicyassignment.md) 资源类型及其相关方法检索适用于每个Azure AD角色的规则。 然后，使用 [Update unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-update.md) API 更新应用于分配给特定Azure AD角色的策略的默认规则或设置。

有关角色设置的详细信息，请参阅[Privileged Identity Management中配置Azure AD角色设置](/azure/active-directory/privileged-identity-management/pim-how-to-change-default-settings)。

## <a name="pim-and-identity-security-with-zero-trust"></a>具有零信任的 PIM 和标识安全性

PIM API 支持组织采用零信任方法保护组织中的标识。 有关零信任的详细信息，请参阅[使用零信任保护标识](/security/zero-trust/deploy/identity)。

## <a name="permissions-and-privileges"></a>权限和权限

若要使用管理员操作调用 [Create roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md) 和 [Create roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md) API，调用用户必须：
+ 具有 *全局管理员* 或 *特权角色管理员* 角色
+ 被授予以下权限之一：
  + RoleAssignmentSchedule.ReadWrite.Directory
  + RoleEligibilitySchedule.ReadWrite.Directory
  + RoleManagement.ReadWrite.Directory

还必须为主体分配适当的权限来检索其角色分配和可变性，或使用用户操作调用 [Create roleAssignmentScheduleRequests](../api/rbacapplication-post-roleassignmentschedulerequests.md) 和 [Create roleEligibilityScheduleRequests](../api/rbacapplication-post-roleeligibilityschedulerequests.md) API。

有关调用 PIM API 的权限的详细信息，请参阅 [Microsoft Graph权限参考：角色管理权限](/graph/permissions-reference#role-management-permissions)。

## <a name="licensing"></a>授权

PIM API 需要Azure AD Premium P2许可证。 有关详细信息，请参阅[使用Privileged Identity Management的许可证要求](/azure/active-directory/privileged-identity-management/subscription-requirements)。

## <a name="next-steps"></a>后续步骤

+ [unifiedRoleAssignmentScheduleRequest 资源类型](unifiedroleassignmentschedulerequest.md)
+ [unifiedRoleEligibilityScheduleRequest 资源类型](unifiedroleeligibilityschedulerequest.md)
+ 还可以设置通过 PIM 管理的角色分配和可视性的访问评审。 有关详细信息，请参阅[教程：使用 Privileged Identity Management (PIM) API 分配Azure AD角色](/graph/tutorial-assign-azureadroles)

## <a name="see-also"></a>另请参阅

+ [什么是 Azure AD Privileged Identity Management？](/azure/active-directory/privileged-identity-management/pim-configure)
+ [教程：使用 Privileged Identity Management (PIM) API 分配Azure AD角色](/graph/tutorial-assign-azureadroles)