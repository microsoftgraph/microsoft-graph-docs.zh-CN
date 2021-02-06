---
title: 使用 Azure AD 权利管理 API
description: 通过 Azure AD 权利管理管理对资源（包括组、应用和网站）的访问
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: d2363e60a0eb99388d3da36264802f87bc12ee93
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131528"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>使用 Azure AD 权利管理 API

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) 权限管理可帮助您管理对内部用户和组织外部用户对组、应用程序和 SharePoint Online 网站的访问权限。

通过创建具有用户跨这些资源所需的角色的访问包，并定义可请求访问包的用户的策略以及他们可以分配访问包的多久，您可以管理内部和外部用户访问的生命周期。

权利管理资源类型包括：

- [accessPackage：](accesspackage.md)定义资源角色的集合以及一个或多个用户如何获取对这些资源的访问权限的策略。
- [accessPackageAssignmentPolicy：](accesspackageassignmentpolicy.md)指定主题可通过访问包分配请求或分配访问包的策略。
- [accessPackageAssignmentRequest：](accesspackageassignmentrequest.md)由希望获取访问包分配的用户创建。
- [accessPackageAssignment：](accesspackageassignment.md)一段时间内向特定主题分配访问包。
- [accessPackageAssignmentResourceRole：](accesspackageassignmentresourcerole.md)指示主题通过访问包分配分配的资源特定角色。
- [accessPackageCatalog：](accesspackagecatalog.md)访问包的容器。
- [accessPackageResourceRequest：](accesspackageresourcerequest.md)向访问包目录添加资源的请求。
- [accessPackageResourceEnvironment：](accesspackageresourceenvironment.md)对资源的地理位置的引用。 适用于多地理位置 SharePoint Online 网站。
- [connectedOrganization：](connectedorganization.md)可请求访问的外部用户的已连接组织。
- [entitlementManagementSettings：Azure](entitlementmanagementsettings.md)AD 权利管理的租户范围设置。

有关介绍如何使用权利管理创建内部用户可以自助请求的资源包的教程，请参阅使用 [Microsoft Graph API](/graph/tutorial-access-package-api)创建访问包。

请注意，权利管理功能（包括 API）包含在 Azure AD Premium P2 中。 使用权利管理的租户必须具有有效的已购买或试用 Azure AD Premium P2 或 EMS E5 订阅。

## <a name="methods"></a>方法

下表列出了可用于与与权利管理相关的资源进行交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
| [获取](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | 读取 **entitlementManagementSettings 对象** 的属性。 |
| [更新](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | 更新 **entitlementManagementSettings 对象** 的属性。 |
| [列出 accessPackages](../api/accesspackage-list.md) | [accessPackage](accesspackage.md) 集合 | 检索 **accessPackage 对象** 的列表。 |
| [创建 accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | 创建新的 **accessPackage** 对象。 |
| [获取 accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | 读取 **accessPackage 对象的属性和** 关系。 |
| [更新 accessPackage](../api/accesspackage-update.md)|无 | 更新 **accesspackage 对象** 的属性。 |
| [删除 accessPackage](../api/accesspackage-delete.md) | | 删除 **accessPackage**。 |
| [列出 accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合 | 检索访问 **包的 accessPackageResourceRoleScope** 对象列表。 |
| [创建 accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | 为访问包 **创建新的 accessPackageResourceRoleScope** 对象。 |
| [列出 accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 集合 | 检索 **accessPackageAssignmentPolicy 对象** 的列表。 |
| [创建 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| 创建新的 **accessPackageAssignmentPolicy** 对象。 |
| [获取 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 读取 **accessPackageAssignmentPolicy** 对象的属性和关系。 |
| [更新 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md)|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 更新 **accessPackageAssignmentPolicy 对象** 的属性。 |
| [删除 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | 删除 **accessPackageAssignmentPolicy**。 |
| [列出 accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合 | 检索 **accessPackageAssignmentRequest 对象** 的列表。 |
| [创建 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的 **accessPackageAssignmentRequest**。 |
| [获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 读取 **accessPackageAssignmentRequest** 对象的属性和关系。 |
| [列出 accessPackageAssignments](../api/accesspackageassignment-list.md) | [accessPackageAssignment](accesspackageassignment.md) 集合 | 检索 **accessPackageAssignment 对象** 的列表。 |
| [列出 accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) 集合 | 检索 **accessPackageAssignmentResourceRole 对象** 的列表。 |
| [获取 accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | 检索 **accessPackageAssignmentResourceRole** 对象。 |
| [列出 accessPackageCatalogs](../api/accesspackagecatalog-list.md) | [accessPackageCatalog](accesspackagecatalog.md) 集合 | 检索 **accessPackageCatalogs 对象** 的列表。 |
| [创建 accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | 创建新的 **accessPackageCatalog** 对象。 |
| [获取 accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | 读取 **accessPackageCatalog** 对象的属性和关系。 |
| [更新 accessPackageCatalog](../api/accesspackagecatalog-update.md)|无 | 更新 **accessPackageCatalog 对象** 的属性。 |
| [删除 accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | 删除 **accessPackageCatalog**。 |
| [列出 accessPackageCatalog 资源](../api/accesspackagecatalog-list-accesspackageresources.md) | [accessPackageResource](accesspackageresource.md) 集合 | 检索 **accessPackageResource 对象** 的列表。 |
| [列出 accessPackageCatalog 资源角色](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [accessPackageResourceRole](accesspackageresourcerole.md) 集合 | 检索 **accessPackageResourceRole 对象** 的列表。 |
| [列出 accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | [accessPackageResourceRequest](accesspackageresourcerequest.md) 集合 | 读取 **accessPackageResourceRequest** 对象的属性和关系。 |
| [创建 accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | 创建新的 **accessPackageResourceRequest** 对象。 |
|[列出 accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 集合|检索 [accessPackageResourceEnvironment 对象](../resources/accesspackageresourceenvironment.md) 的列表。|
|[获取 accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|读取 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象的属性和关系。|
| [列出 connectedOrganizations](../api/connectedorganization-list.md) | [connectedOrganization](connectedorganization.md) 集合 | 检索 **connectedOrganization 对象** 的列表。 |
| [创建 connectedOrganization](../api/connectedorganization-post.md) | [connectedOrganization](connectedorganization.md) | 创建新的 **connectedOrganization** 对象。 |
| [获取 connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | 读取 **connectedOrganization 对象的属性和** 关系。 |
| [更新 connectedOrganization](../api/connectedorganization-update.md) |无 | 更新 **connectedOrganization**。 |
| [删除 connectedOrganization](../api/connectedorganization-delete.md) |无 | 删除 **connectedOrganization**。 |
|[列出 internalSponsors](../api/connectedorganization-list-internalsponsors.md) | [directoryObject](directoryobject.md) 集合 | 检索 **connectedOrganization 的内部发起** 人的列表。 |
|[列出 externalSponsors](../api/connectedorganization-list-externalsponsors.md) | [directoryObject](directoryobject.md) 集合 | 检索 **connectedOrganization 的外部发起人** 的列表。 |
|[添加 internalSponsors](../api/connectedorganization-post-internalsponsors.md) | 无 | 将用户或组添加到 **connectedOrganization 的内部** 发起人。 |
|[添加 externalSponsors](../api/connectedorganization-post-externalsponsors.md) | 无 | 将用户或组添加到 **connectedOrganization 的外部** 发起人。 |
|[删除 internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | 无 | 从 **connectedOrganization** 的内部发起人中删除用户或组。 |
|[删除 externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | 无 | 从 **connectedOrganization** 的外部发起人中删除用户或组。 |

## <a name="types"></a>类型

- [requestorSettings](requestorsettings.md)、 [approvalSettings](approvalsettings.md)、 [问题和](accesspackagequestion.md) [assignmentReviewSettings](assignmentreviewsettings.md) - 在 [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 中用于指定谁可以请求、批准以及谁审阅该策略上的访问包分配请求。
- [approvalStage](approvalstage.md) - 在 [approvalSettings](approvalsettings.md) 中用于指定主要、备份和升级审批者。
- [userSet](userset.md)子类型[singleUser](singleuser.md)、groupMembers、connectedOrganizationMembers、requestorManager、internalSponsors 和[](connectedorganizationmembers.md)[](requestormanager.md)[externalSponsors](externalsponsors.md) - 用于[requestorSettings、approvalStage](requestorsettings.md)和[assignmentReviewSettings。](assignmentreviewsettings.md) [](groupmembers.md) [](internalsponsors.md) [](approvalstage.md)
- [accessPackageSubject](accesspackagesubject.md) - 在 [accessPackageAssignment](accesspackageassignment.md) 中用作具有访问包分配的主题用户。
- [identitySource](identitysource.md) - 用于[connectedOrganization](connectedorganization.md)，azureActiveDirectoryTenant ， [domainIdentitySource](domainidentitysource.md)或[externalDomainFederation](externaldomainfederation.md)之一。 [](azureactivedirectorytenant.md)

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
