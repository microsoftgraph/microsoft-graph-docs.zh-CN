---
title: 使用 Azure AD 权利管理 API
description: 通过 Azure AD 权利管理管理对资源（包括组、应用和网站）的访问
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: b08d44a0aaa1b99d2937fd68c1dc822328f7bdb3
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764792"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>使用 Azure AD 权利管理 API

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) 权限管理可帮助你管理内部用户以及组织外部用户对组、应用程序和 SharePoint Online 网站的访问权限。

通过创建具有用户跨这些资源所需的角色的访问包，并定义哪些人可以请求访问包以及他们可以向访问包分配多久的策略，你可以管理内部和外部用户访问的生命周期。

权利管理资源类型包括：

- [accessPackage：](accesspackage.md)定义资源角色的集合以及一个或多个用户如何获取对这些资源的访问权限的策略。
- [accessPackageAssignmentPolicy：](accesspackageassignmentpolicy.md)指定主题可以通过访问包分配请求或分配访问包的策略。
- [accessPackageAssignmentRequest：](accesspackageassignmentrequest.md)由希望获取访问包分配的用户创建。
- [accessPackageAssignment：](accesspackageassignment.md)在一段时间内向特定主题分配访问包。
- [accessPackageAssignmentResourceRole：](accesspackageassignmentresourcerole.md)指示主题通过访问包分配分配的资源特定角色。
- [accessPackageCatalog：](accesspackagecatalog.md)访问包的容器。
- [accessPackageResourceRequest：](accesspackageresourcerequest.md)向访问包目录添加资源的请求。
- [accessPackageResourceEnvironment：](accesspackageresourceenvironment.md)对资源的地理位置的引用。 适用于多地理位置SharePoint在线网站。
- [connectedOrganization：](connectedorganization.md)可请求访问的外部用户的已连接组织。
- [entitlementManagementSettings：Azure](entitlementmanagementsettings.md)AD 权利管理的租户范围设置。
- [approval](approval.md)：表示与访问包请求相关的决策。

此外，可通过权利管理角色定义管理特定于权利管理的角色[分配。](unifiedroledefinition.md)

有关介绍如何使用权利管理创建内部用户可以自助请求的资源包的教程，请参阅使用 Microsoft Graph [API 创建访问包](/graph/tutorial-access-package-api)。

请注意，权利管理功能（包括 API）包含在Azure AD Premium P2。 使用权利管理的租户必须拥有有效的已购买或试用Azure AD Premium P2 EMS E5 订阅。

## <a name="methods"></a>方法

下表列出了可用于与权利管理相关资源进行交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
| [Get](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | 读取 **entitlementManagementSettings 对象** 的属性。 |
| [更新](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | 更新 **entitlementManagementSettings 对象** 的属性。 |
| [列出 accessPackages](../api/accesspackage-list.md) | [accessPackage](accesspackage.md) 集合 | 检索 **accessPackage 对象** 的列表。 |
| [创建 accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | 创建新的 **accessPackage** 对象。 |
| [获取 accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | 读取 **accessPackage 对象的属性和** 关系。 |
| [更新 accessPackage](../api/accesspackage-update.md)|无 | 更新 **accesspackage 对象** 的属性。 |
| [删除 accessPackage](../api/accesspackage-delete.md) | | 删除 **accessPackage**。 |
| [FilterByCurrentUser](../api/accesspackage-filterbycurrentuser.md) | [accessPackage](accesspackage.md) 集合 | 检索在已登录用户上筛选的 **accessPackage** 对象列表。 |
| [列出 accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合 | 检索访问 **包的 accessPackageResourceRoleScope** 对象列表。 |
| [创建 accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | 为访问包 **创建新的 accessPackageResourceRoleScope** 对象。 |
| [列出 incompatibleAccessPackages](../api/accesspackage-list-incompatibleaccesspackages.md) | [accessPackage](accesspackage.md) 集合 | 检索此访问包 **的不兼容 accesspackage** 对象的列表。 |
| [将 accessPackage 添加到 incompatibleAccessPackages](../api/accesspackage-post-incompatibleaccesspackage.md) | 无 | 添加一个链接以指示另一 **个 accesspackage** 与指定的访问包不兼容。 |
| [从 incompatibleAccessPackages 中删除 accessPackage](../api/accesspackage-delete-incompatibleaccesspackage.md) | 无 | 删除指示 **accesspackage 不兼容** 的链接。 |
| [列出 incompatibleGroups](../api/accesspackage-list-incompatiblegroups.md) | [组](group.md) 集合 | 检索此 **访问包的** 不兼容组对象的列表。 |
| [将组添加到 incompatibleGroups](../api/accesspackage-post-incompatiblegroup.md) | 无 | 添加链接以指示组的成员身份 **与** 指定的访问包不兼容。 |
| [从 incompatibleGroups 中删除组](../api/accesspackage-delete-incompatiblegroup.md) | 无 | 删除指示组成员身份 **不兼容** 的链接。|
| [列出 accessPackagesIncompatibleWith](../api/accesspackage-list-accesspackagesincompatiblewith.md) | [accessPackage](accesspackage.md) 集合 | 检索  **accesspackage 对象** 的列表，这些对象将此访问包列出为不兼容。 |
| [列出 accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合 | 检索 **accessPackageAssignmentPolicy 对象** 的列表。 |
| [创建 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| 创建新的 **accessPackageAssignmentPolicy** 对象。 |
| [获取 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 读取 **accessPackageAssignmentPolicy 对象的属性和** 关系。 |
| [更新 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 更新 **accessPackageAssignmentPolicy 对象** 的属性。 |
| [删除 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | 删除 **accessPackageAssignmentPolicy**。 |
| [列出 accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合 | 检索 **accessPackageAssignmentRequest 对象** 的列表。 |
| [创建 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的 **accessPackageAssignmentRequest**。 |
| [获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 读取 **accessPackageAssignmentRequest** 对象的属性和关系。 |
| [删除 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |无 | 删除 **accessPackageAssignmentRequest**。 |
|[FilterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|检索已登录 **用户筛选的 accessPackageAssignmentRequest** 对象列表。|
|[取消](../api/accesspackageassignmentrequest-cancel.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|取消 **处于可取消状态的访问PackageAssignmentRequest** 对象：、、、。 `accepted` `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated`|
| [列出 accessPackageAssignments](../api/accesspackageassignment-list.md) | [accessPackageAssignment](accesspackageassignment.md) 集合 | 检索 **accessPackageAssignment 对象** 的列表。 |
|[FilterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) 集合|检索在登录用户上筛选的 **accessPackageAssignment** 对象列表。|
| [列出 accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合 | 检索 **accessPackageAssignmentResourceRole 对象** 的列表。 |
| [获取 accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | 检索 **accessPackageAssignmentResourceRole** 对象。 |
| [列出 accessPackageCatalogs](../api/accesspackagecatalog-list.md) | [accessPackageCatalog](accesspackagecatalog.md) 集合 | 检索 **accessPackageCatalogs 对象** 的列表。 |
| [创建 accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | 创建新的 **accessPackageCatalog** 对象。 |
| [获取 accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | 读取 **accessPackageCatalog 对象的属性和** 关系。 |
| [更新 accessPackageCatalog](../api/accesspackagecatalog-update.md)|无 | 更新 **accessPackageCatalog 对象** 的属性。 |
| [删除 accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | 删除 **accessPackageCatalog**。 |
| [列出 accessPackageCatalog 资源](../api/accesspackagecatalog-list-accesspackageresources.md) | [accessPackageResource](accesspackageresource.md) 集合 | 检索 **accessPackageResource 对象** 的列表。 |
| [列出 accessPackageCatalog 资源角色](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [accessPackageResourceRole](accesspackageresourcerole.md) 集合 | 检索 **accessPackageResourceRole 对象** 的列表。 |
| [列出 accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | [accessPackageResourceRequest](accesspackageresourcerequest.md) 集合 | 读取 **accessPackageResourceRequest 对象的属性和** 关系。 |
| [创建 accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | 创建新的 **accessPackageResourceRequest** 对象。 |
|[列出 accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 集合|检索 [accessPackageResourceEnvironment 对象](../resources/accesspackageresourceenvironment.md) 的列表。|
|[获取 accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|读取 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象的属性和关系。|
| [列出 connectedOrganizations](../api/connectedorganization-list.md) | [connectedOrganization](connectedorganization.md) 集合 | 检索 **connectedOrganization 对象** 的列表。 |
| [创建 connectedOrganization](../api/connectedorganization-post.md) | [connectedOrganization](connectedorganization.md) | 创建新的 **connectedOrganization** 对象。 |
| [获取 connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | 读取 **connectedOrganization 对象的属性和** 关系。 |
| [更新 connectedOrganization](../api/connectedorganization-update.md) |无 | 更新 **connectedOrganization**。 |
| [删除 connectedOrganization](../api/connectedorganization-delete.md) |无 | 删除 **connectedOrganization**。 |
|[列出 internalSponsors](../api/connectedorganization-list-internalsponsors.md) | [directoryObject](directoryobject.md) 集合 | 检索 **connectedOrganization 的内部发起人** 的列表。 |
|[列出 externalSponsors](../api/connectedorganization-list-externalsponsors.md) | [directoryObject](directoryobject.md) 集合 | 检索 **connectedOrganization 的外部发起** 人的列表。 |
|[添加 internalSponsors](../api/connectedorganization-post-internalsponsors.md) | 无 | 将用户或组添加到 **connectedOrganization 的内部发起** 人。 |
|[添加 externalSponsors](../api/connectedorganization-post-externalsponsors.md) | 无 | 将用户或组添加到 **connectedOrganization 的外部** 发起人。 |
|[删除 internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | 无 | 从 **connectedOrganization 的内部发起人中删除用户或** 组。 |
|[获取审批](../api/approval-get.md) | [审批](approval.md) | 检索 **审批对象的属性** 。 |
|[列出 approvalSteps](../api/approval-list-steps.md) | [approvalStep](approvalstep.md) 集合 | 列出 **与审批对象关联的 approvalStep** **对象。** |
|[获取审批步骤](../api/approvalstep-get.md) | [approvalStep](approvalstep.md) | 检索 **approvalStep 对象** 的属性。 |
|[更新 approvalStep](../api/approvalstep-update.md) | 无 | 对 approvalStep 对象应用 **批准或拒绝** 决定。 |


## <a name="types"></a>类型

- [requestorSettings](requestorsettings.md) [、approvalSettings、questions](approvalsettings.md)和[assignmentReviewSettings](assignmentreviewsettings.md) - 在[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)中用于指定谁可以请求、批准以及谁审阅该策略上的访问包分配请求。 [](accesspackagequestion.md)
- [approvalStage](approvalstage.md) - 在 [approvalSettings](approvalsettings.md) 中用于指定主要、备份和升级审批者。
- [approvalStep](approvalstep.md) - 在 [审批中用于](approval.md) 区分不同的审批步骤。
- [userSet](userset.md)子类型 singleUser、groupMembers、connectedOrganizationMembers、requestorManager、internalSponsors 和[](groupmembers.md)[](requestormanager.md)[externalSponsors](externalsponsors.md) - 在[](singleuser.md) [requestorSettings、approvalStage、approvalStep](requestorsettings.md)和[assignmentReviewSettings](assignmentreviewsettings.md)中使用。 [](connectedorganizationmembers.md) [](internalsponsors.md) [](approvalstage.md) [](approvalstep.md)
- [accessPackageSubject](accesspackagesubject.md) - 在 [accessPackageAssignment](accesspackageassignment.md) 中用作具有访问包分配的主题用户。
- [identitySource](identitysource.md) - 用于[connectedOrganization](connectedorganization.md)，azureActiveDirectoryTenant 、 [domainIdentitySource](domainidentitysource.md)或[externalDomainFederation 之一](externaldomainfederation.md)。 [](azureactivedirectorytenant.md)

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
