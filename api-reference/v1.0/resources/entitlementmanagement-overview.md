---
title: 使用 Azure AD权限管理 API
description: 通过权利管理管理对资源（包括组、应用和Azure AD的访问）
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 38d30da6d55ebdff4abb55d584b4c0cb7d59a9fa
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651567"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>使用 Azure AD权限管理 API

命名空间：microsoft.graph

Azure Active Directory (Azure AD) 管理可帮助您管理内部用户以及组织外部SharePoint组、应用程序和 SharePoint Online 网站的访问权限。

通过创建具有用户跨这些资源所需的角色的访问包，并定义哪些人可以请求访问包以及他们可以向访问包分配多久的策略，你可以管理内部和外部用户访问的生命周期。

权利管理资源类型包括：

- [accessPackage：](accesspackage.md)定义资源角色的集合以及一个或多个用户如何获取对这些资源的访问权限的策略。
- accessPackageAssignmentPolicy：指定主题可以通过访问包分配请求或分配访问包的策略。
- [accessPackageAssignmentRequest：](accesspackageassignmentrequest.md)由希望获取访问包分配的用户创建。
- [accessPackageAssignment：](accesspackageassignment.md)在一段时间内向特定主题分配访问包。
- [accessPackageCatalog：](accesspackagecatalog.md)访问包的容器。
- [connectedOrganization：](connectedorganization.md)可请求访问的外部用户的已连接组织。
- [entitlementManagementSettings：](entitlementmanagementsettings.md)用于管理Azure AD范围的设置。
- [approval](approval.md)：表示与访问包请求相关的决策。

请注意，权利管理功能（包括 API）包含在Azure AD Premium P2。 使用权利管理的租户必须拥有有效的已购买或试用Azure AD Premium P2 EMS E5 订阅。

下表列出了可用于与权利管理相关资源进行交互的方法。

## <a name="methods"></a>方法

| 方法   | 返回类型 |说明|
|:---------------|:--------|:----------|
| [获取](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | 读取 **entitlementManagementSettings 对象** 的属性。 |
| [更新](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | 更新 **entitlementManagementSettings 对象** 的属性。 |
| [列出 accessPackages](../api/entitlementmanagement-list-accesspackages.md) | [accessPackage](accesspackage.md) 集合 | 检索 **accessPackage 对象** 的列表。 |
| [创建 accessPackage](../api/entitlementmanagement-post-accesspackages.md) | [accessPackage](accesspackage.md) | 创建新的 **accessPackage** 对象。 |
| [获取 accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | 读取 **accessPackage 对象的属性和** 关系。 |
| [更新 accessPackage](../api/accesspackage-update.md)|无 | 更新 **accesspackage 对象** 的属性。 |
| [删除 accessPackage](../api/accesspackage-delete.md) | | 删除 **accessPackage**。 |
| [FilterByCurrentUser](../api/accesspackage-filterbycurrentuser.md) | [accessPackage](accesspackage.md) 集合 | 检索在已登录用户上筛选的 **accessPackage** 对象列表。 |
| [列出 accessPackageAssignmentRequests](../api/entitlementmanagement-list-assignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) 集合 | 检索 **accessPackageAssignmentRequest 对象** 的列表。 |
| [创建 accessPackageAssignmentRequest](../api/entitlementmanagement-post-assignmentrequests.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的 **accessPackageAssignmentRequest** 对象。 |
| [获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 读取 **accessPackageAssignmentRequest** 对象的属性和关系。 |
| [删除 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-delete.md) |无 | 删除 **accessPackageAssignmentRequest**。 |
|[FilterByCurrentUser](../api/accesspackageassignmentrequest-filterbycurrentuser.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|检索已登录 **用户筛选的 accessPackageAssignmentRequest** 对象列表。|
|[取消](../api/accesspackageassignmentrequest-cancel.md)|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|取消 **处于可取消状态的访问PackageAssignmentRequest** 对象：、、、。 `accepted` `pendingApproval` `pendingNotBefore` `pendingApprovalEscalated`|
| [列出 accessPackageAssignments](../api/entitlementmanagement-list-assignments.md) | [accessPackageAssignment](accesspackageassignment.md) 集合 | 检索 **accessPackageAssignment 对象** 的列表。 |
|[FilterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) 集合|检索在登录用户上筛选的 **accessPackageAssignment** 对象列表。|
| [列出 accessPackageCatalogs](../api/entitlementmanagement-list-catalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) 集合 | 检索 **accessPackageCatalogs 对象** 的列表。 |
| [创建 accessPackageCatalog](../api/entitlementmanagement-post-catalogs.md) | [accessPackageCatalog](accesspackagecatalog.md) | 创建新的 **accessPackageCatalog** 对象。 |
| [获取 accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | 读取 **accessPackageCatalog 对象的属性和** 关系。 |
| [更新 accessPackageCatalog](../api/accesspackagecatalog-update.md)|无 | 更新 **accessPackageCatalog 对象** 的属性。 |
| [删除 accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | 删除 **accessPackageCatalog**。 |
| [列出 connectedOrganizations](../api/entitlementmanagement-list-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) 集合 | 检索 **connectedOrganization 对象** 的列表。 |
| [创建 connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md) | [connectedOrganization](connectedorganization.md) | 创建新的 **connectedOrganization** 对象。 |
| [获取 connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | 读取 **connectedOrganization 对象的属性和** 关系。 |
| [更新 connectedOrganization](../api/connectedorganization-update.md) |无 | 更新 **connectedOrganization**。 |
| [删除 connectedOrganization](../api/connectedorganization-delete.md) |无 | 删除 **connectedOrganization**。 |
|[列出 internalSponsors](../api/connectedorganization-list-internalsponsors.md) | [directoryObject](directoryobject.md) collection | 检索 **connectedOrganization 的内部发起人** 的列表。 |
|[列出 externalSponsors](../api/connectedorganization-list-externalsponsors.md) | [directoryObject](directoryobject.md) collection | 检索 **connectedOrganization 的外部发起** 人的列表。 |
|[添加 internalSponsors](../api/connectedorganization-post-internalsponsors.md) | 无 | 将用户或组添加到 **connectedOrganization 的内部发起** 人。 |
|[添加 externalSponsors](../api/connectedorganization-post-externalsponsors.md) | 无 | 将用户或组添加到 **connectedOrganization 的外部** 发起人。 |
|[删除 internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | 无 | 从 **connectedOrganization 的内部发起人中删除用户或** 组。 |
|[删除 externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | 无 | 从 **connectedOrganization 的外部发起人中删除用户或** 组。 |

## <a name="see-also"></a>另请参阅

- [什么是Azure AD权限管理？](/azure/active-directory/governance/entitlement-management-overview)
- [subjectSet](subjectset.md)子类型 singleUser、groupMembers、connectedOrganizationMembers、requestorManager、internalSponsors 和[](requestormanager.md)[externalSponsors](externalsponsors.md)。 [](singleuser.md) [](groupmembers.md) [](connectedorganizationmembers.md) [](internalsponsors.md)
- [accessPackageSubject](accesspackagesubject.md) - 在 [accessPackageAssignment](accesspackageassignment.md) 中用作具有访问包分配的主题用户。
- [identitySource](identitysource.md) - 用于[connectedOrganization](connectedorganization.md)，azureActiveDirectoryTenant 、 [domainIdentitySource](domainidentitysource.md)或[externalDomainFederation 之一](externaldomainfederation.md)。 [](azureactivedirectorytenant.md)


