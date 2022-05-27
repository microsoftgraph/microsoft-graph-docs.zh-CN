---
title: 使用 Azure AD 权利管理 API
description: 通过 Azure AD 权利管理控制对包括组、应用和站点在内的资源的访问
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 520d786906963250024121144865cfcf15e07560
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694733"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>使用 Azure AD 权利管理 API

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) 权利管理可以帮助你管理对内部用户以及组织外部用户的组、应用程序和SharePoint Online 网站的访问权限。

通过使用用户在这些资源中需要具有的角色创建访问包，并为谁可以请求访问包以及他们可以分配访问包多长时间定义策略，可以控制内部和外部用户的访问生命周期。

权利管理资源类型包括：

- [accessPackage](accesspackage.md)：定义资源角色的集合以及一个或多个用户如何获取对这些资源的访问权限的策略。
- [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)：指定通过访问包分配来请求或分配访问包的主题的策略。
- [accessPackageAssignmentRequest](accesspackageassignmentrequest.md)：由希望获取访问包分配的用户创建。
- [accessPackageAssignment](accesspackageassignment.md)：向特定主题分配访问包一段时间。
- [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)：指示通过访问包分配分配主题的特定于资源的角色。
- [accessPackageCatalog](accesspackagecatalog.md)：用于访问包的容器。
- [accessPackageResource](accesspackageresource.md)：对与访问包目录关联的资源的引用。
- [accessPackageResourceRequest](accesspackageresourcerequest.md)：向访问包目录添加资源的请求。
- [accessPackageResourceEnvironment](accesspackageresourceenvironment.md)：对资源地理位置的引用。 适用于多地理位置SharePoint联机网站。
- [connectedOrganization](connectedorganization.md)：可请求访问权限的外部用户的已连接组织。
- [entitlementManagementSettings](entitlementmanagementsettings.md)：Azure AD 权利管理的租户范围设置。
- [审批](approval.md)：表示与访问包请求关联的决策。

此外，可以通过权利管理角色定义来管理特定于权利管理 [的角色的角色](unifiedroledefinition.md)分配。

有关演示如何使用权利管理创建内部用户可以自助请求的资源包的教程，请参阅[使用 Microsoft Graph API 创建访问包](/graph/tutorial-access-package-api)。

请注意，权利管理功能（包括 API）包含在Azure AD Premium P2中。 使用权利管理的租户必须具有有效的购买或试用Azure AD Premium P2或 EMS E5 订阅。 有关权利管理功能的许可证要求的详细信息，请参阅 [权利管理许可证要求](/azure/active-directory/governance/entitlement-management-overview#license-requirements)。

## <a name="methods"></a>方法

下表列出了可用于与权利管理相关资源交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
| [获取](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | 读取 **entitlementManagementSettings 对象的** 属性。 |
| [更新](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | 更新 **entitlementManagementSettings 对象的** 属性。 |
| [列出 accessPackages](../api/entitlementmanagement-list-accesspackages.md) | [accessPackage](accesspackage.md) 集合 | 检索 **accessPackage** 对象的列表。 |
| [创建 accessPackage](../api/entitlementmanagement-post-accesspackages.md) | [accessPackage](accesspackage.md) | 创建新的 **accessPackage** 对象。 |
| [获取 accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | 读取 **accessPackage** 对象的属性和关系。 |
| [更新 accessPackage](../api/accesspackage-update.md)|无 | 更新 **accesspackage** 对象的属性。 |
| [删除 accessPackage](../api/accesspackage-delete.md) | | 删除 **accessPackage**。 |
| [FilterByCurrentUser](../api/accesspackage-filterbycurrentuser.md) | [accessPackage](accesspackage.md) 集合 | 检索已登录用户上筛选的 **accessPackage** 对象的列表。 |
| [列出 accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合 | 检索访问包的 **accessPackageResourceRoleScope** 对象列表。 |
| [创建 accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | 为访问包创建新的 **accessPackageResourceRoleScope** 对象。 |
| [列出不兼容的AccessPackages](../api/accesspackage-list-incompatibleaccesspackages.md) | [accessPackage](accesspackage.md) 集合 | 检索此访问包的不兼容 **访问包** 对象的列表。 |
| [将 accessPackage 添加到不兼容的AccessPackages](../api/accesspackage-post-incompatibleaccesspackage.md) | 无 | 添加一个链接，指示另一 **个 accesspackage** 与指定的访问包不兼容。 |
| [从不兼容的AccessPackages中删除 accessPackage](../api/accesspackage-delete-incompatibleaccesspackage.md) | 无 | 删除指示 **访问包** 不兼容的链接。 |
| [列出不兼容组](../api/accesspackage-list-incompatiblegroups.md) | [group](group.md) 集合 | 检索此访问包的不兼容 **组** 对象的列表。 |
| [将组添加到不兼容组](../api/accesspackage-post-incompatiblegroup.md) | 无 | 添加一个链接以指示 **组** 的成员身份与指定的访问包不兼容。 |
| [从不兼容组中删除组](../api/accesspackage-delete-incompatiblegroup.md) | 无 | 删除指示 **组** 成员身份不兼容的链接。|
| [列出 accessPackagesIncompatibleWith](../api/accesspackage-list-accesspackagesincompatiblewith.md) | [accessPackage](accesspackage.md) 集合 | 检索  **Accesspackage** 对象的列表，这些对象将此访问包列为不兼容。 |
| [列出 accessPackageAssignmentPolicies](../api/entitlementmanagement-list-accesspackageassignmentpolicies.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合 | 检索 **accessPackageAssignmentPolicy** 对象的列表。 |
| [创建 accessPackageAssignmentPolicy](../api/entitlementmanagement-post-accesspackageassignmentpolicies.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| 创建新的 **accessPackageAssignmentPolicy** 对象。 |
| [获取 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 读取 **accessPackageAssignmentPolicy** 对象的属性和关系。 |
| [更新 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 更新 **accessPackageAssignmentPolicy 对象的** 属性。 |
| [删除 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | 删除 **accessPackageAssignmentPolicy**。 |
| [列出 accessPackageAssignmentRequests](../api/entitlementmanagement-list-accesspackageassignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合 | 检索 **accessPackageAssignmentRequest** 对象的列表。 |
| [创建 accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的 **accessPackageAssignmentRequest**。 |
| [获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 读取 **accessPackageAssignmentRequest** 对象的属性和关系。 |
| [删除 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |无 | 删除 **accessPackageAssignmentRequest**。 |
|[FilterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|检索已登录用户上筛选的 **accessPackageAssignmentRequest** 对象的列表。|
|[取消](../api/accesspackageassignmentrequest-cancel.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|取消处于可取消状态 **的 accessPackageAssignmentRequest** 对象： `accepted`， ， `pendingApproval``pendingNotBefore`， . `pendingApprovalEscalated`|
| [列出 accessPackageAssignments](../api/entitlementmanagement-list-accesspackageassignments.md) | [accessPackageAssignment](accesspackageassignment.md) 集合 | 检索 **accessPackageAssignment 对象的** 列表。 |
|[FilterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) 集合|检索已登录用户上筛选的 **accessPackageAssignment** 对象的列表。|
| [重新处理](../api/accesspackageassignment-reprocess.md) | 无 | 自动重新评估并强制执行特定访问包的用户分配。|
| [additionalAccess](../api/accesspackageassignment-additionalaccess.md) [accessPackageAssignment](../resources/accesspackageassignment.md) 集合|检索分配到不兼容访问包的用户的 **accessPackageAssignment** 对象列表。|
| [列出 accessPackageAssignmentResourceRoles](../api/entitlementmanagement-list-accesspackageassignmentresourceroles.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合 | 检索 **accessPackageAssignmentResourceRole** 对象的列表。 |
| [获取 accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | 检索 **accessPackageAssignmentResourceRole** 对象。 |
| [列出 accessPackageCatalogs](../api/entitlementmanagement-list-accesspackagecatalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) 集合 | 检索 **accessPackageCatalogs 对象的** 列表。 |
| [创建 accessPackageCatalog](../api/entitlementmanagement-post-accesspackagecatalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | 创建新的 **accessPackageCatalog** 对象。 |
| [获取 accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | 读 **取 accessPackageCatalog** 对象的属性和关系。 |
| [更新 accessPackageCatalog](../api/accesspackagecatalog-update.md)|无 | 更新 **accessPackageCatalog** 对象的属性。 |
| [删除 accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | 删除 **accessPackageCatalog**。 |
| [列出 accessPackageCatalog 资源](../api/accesspackagecatalog-list-accesspackageresources.md) | [accessPackageResource](accesspackageresource.md) 集合 | 检索 **accessPackageResource** 对象的列表。 |
| [列出 accessPackageCatalog 资源角色](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [accessPackageResourceRole](accesspackageresourcerole.md) 集合 | 检索 **accessPackageResourceRole 对象的** 列表。 |
| [列出 accessPackageResourceRequests](../api/entitlementmanagement-list-accesspackageresourcerequests.md) | [accessPackageResourceRequest](accesspackageresourcerequest.md) 集合 | 读 **取 accessPackageResourceRequest** 对象的属性和关系。 |
| [创建 accessPackageResourceRequest](../api/entitlementmanagement-post-accesspackageresourcerequests.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | 创建新的 **accessPackageResourceRequest** 对象。 |
|[列出 accessPackageResourceEnvironments](../api/entitlementmanagement-list-accesspackageresourceenvironment.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 集合|检索 [accessPackageResourceEnvironment 对象的](../resources/accesspackageresourceenvironment.md) 列表。|
|[获取 accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|读取 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象的属性和关系。|
| [列出 connectedOrganizations](../api/entitlementmanagement-list-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) 集合 | 检索 **connectedOrganization** 对象的列表。 |
| [创建 connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) | 创建新的 **connectedOrganization** 对象。 |
| [获取 connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | 读取 **connectedOrganization** 对象的属性和关系。 |
| [更新 connectedOrganization](../api/connectedorganization-update.md) |无 | 更新 **connectedOrganization**。 |
| [删除 connectedOrganization](../api/connectedorganization-delete.md) |无 | 删除 **connectedOrganization**。 |
|[列出 internalSponsors](../api/connectedorganization-list-internalsponsors.md) | [directoryObject](directoryobject.md) 集合 | 检索 **connectedOrganization 的** 内部发起人的列表。 |
|[列出 externalSponsors](../api/connectedorganization-list-externalsponsors.md) | [directoryObject](directoryobject.md) collection | 检索 **connectedOrganization 的** 外部发起人的列表。 |
|[添加 internalSponsors](../api/connectedorganization-post-internalsponsors.md) | 无 | 将用户或组添加到 **connectedOrganization 的** 内部发起人。 |
|[添加 externalSponsors](../api/connectedorganization-post-externalsponsors.md) | 无 | 将用户或组添加到 **connectedOrganization 的** 外部发起人。 |
|[删除 internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | 无 | 从 **connectedOrganization 的** 内部发起人中删除用户或组。 |
|[获取批准](../api/approval-get.md) | “[审批](approval.md)” | 检索 **审批** 对象的属性。 |
|[List approvalSteps](../api/approval-list-steps.md) | [approvalStep](approvalstep.md) 集合 | 列出与 **审批** 对象关联的 **approvalStep** 对象。 |
|[Get approvalStep](../api/approvalstep-get.md) | [approvalStep](approvalstep.md) | 检索 **approvalStep** 对象的属性。 |
|[Update approvalStep](../api/approvalstep-update.md) | 无 | 对 **approvalStep** 对象应用批准或拒绝决策。 |


## <a name="types"></a>类型

- [requestorSettings](requestorsettings.md)、 [approvalSettings](approvalsettings.md)、 [questions](accesspackagequestion.md) and [assignmentReviewSettings](assignmentreviewsettings.md) - 在 [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 中使用，用于指定谁可以请求、谁批准以及谁对该策略的访问包分配请求进行评审。
- [approvalStage](approvalstage.md) - 在 [approvalSettings](approvalsettings.md) 中用于指定主要、备份和升级审批者。
- [approvalStep](approvalstep.md) - 用于 [审批](approval.md) 以区分不同的审批步骤。
- [userSet](userset.md) 子类型 [singleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [connectedOrganizationMembers](connectedorganizationmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md) 和 [externalSponsors](externalsponsors.md) - 用于 [requestorSettings](requestorsettings.md)、 [approvalStage](approvalstage.md)、 [approvalStep](approvalstep.md) 和 [assignmentReviewSettings](assignmentreviewsettings.md)。
- [accessPackageSubject](accesspackagesubject.md) - 在 [accessPackageAssignment](accesspackageassignment.md) 中用作具有访问包分配的主题用户。
- [identitySource](identitysource.md) - 用于 [connectedOrganization](connectedorganization.md)、 [azureActiveDirectoryTenant](azureactivedirectorytenant.md)、 [crossCloudAzureActiveDirectoryTenant](crosscloudazureactivedirectorytenant.md)、 [domainIdentitySource](domainidentitysource.md) 或 [externalDomainFederation](externaldomainfederation.md) 之一。

## <a name="see-also"></a>另请参阅

 - [什么是 Azure AD 权利管理？](/azure/active-directory/governance/entitlement-management-overview)



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
