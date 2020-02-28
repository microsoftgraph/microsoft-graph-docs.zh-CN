---
title: 使用 Azure AD 权限管理 API
description: 通过 Azure AD 权限管理控制对资源（包括组、应用和网站）的访问
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 7e255a68d46e810d22e26d167dbe3ef5a6714496
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331316"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>使用 Azure AD 权限管理 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory （Azure AD）权限管理可帮助您管理对组、应用程序和 SharePoint Online 网站的访问权限，以供内部用户和组织外部的用户使用。

通过创建具有用户需要跨这些资源的角色的访问包，以及为可以请求访问包的人员定义策略以及为谁分配对访问包的分配的时间，可以控制内部和的访问的生命周期外部用户。

"权限管理" 资源类型包括：

- [accessPackage](accesspackage.md)：定义了资源角色的集合，以及一个或多个用户可以获取这些资源的访问权限的策略。
- [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)：指定通过访问包分配，主题可能请求或为其分配访问包的策略。
- [accessPackageAssignmentRequest](accesspackageassignmentrequest.md)：希望获取访问包分配的用户创建的。
- [accessPackageAssignment](accesspackageassignment.md)：对特定主题的访问包分配在一段时间内。
- [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)：指示通过访问包分配为主题分配的特定于资源的角色。
- [accessPackageCatalog](accesspackagecatalog.md)：访问包的容器。
- [accessPackageResourceRequest](accesspackageresourcerequest.md)：将资源添加到访问包目录的请求。

请注意，"权限管理" 功能（包括 API）包含在 Azure AD Premium P2 中。 使用权限管理的租户必须具有有效的已购买或试用版 Azure AD Premium P2 或 EMS E5 订阅。

## <a name="methods"></a>Methods

下表列出了可用于与与权限管理相关的资源进行交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
| [列出 accessPackages](../api/accesspackage-list.md) | [accessPackage](accesspackage.md)集合 | 检索**accessPackage**对象的列表。 |
| [创建 accessPackage](../api/accesspackage-post.md) | [accessPackage](accesspackage.md) | 创建新的**accessPackage**对象。 |
| [获取 accessPackage](../api/accesspackage-get.md) | [accessPackage](accesspackage.md) | 读取**accessPackage**对象的属性和关系。 |
| [删除 accessPackage](../api/accesspackage-delete.md) | | 删除**accessPackage**。 |
| [列出 accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)集合 | 检索访问包的**accessPackageResourceRoleScope**对象的列表。 |
| [创建 accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | 为 access 包创建一个新的**accessPackageResourceRoleScope**对象。 |
| [列出 accessPackageAssignmentPolicies](../api/accesspackageassignmentpolicy-list.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)集合 | 检索**accessPackageAssignmentPolicy**对象的列表。 |
| [创建 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-post.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| 创建新的**accessPackageAssignmentPolicy**对象。 |
| [获取 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) | [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) | 读取**accessPackageAssignmentPolicy**对象的属性和关系。 |
| [删除 accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-delete.md) | | 删除**accessPackageAssignmentPolicy**。 |
| [列出 accessPackageAssignmentRequests](../api/accesspackageassignmentrequest-list.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md)集合 | 检索**accessPackageAssignmentRequest**对象的列表。 |
| [创建 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 创建新的**accessPackageAssignmentRequest**。 |
| [获取 accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-get.md) | [accessPackageAssignmentRequest](accesspackageassignmentrequest.md) | 读取**accessPackageAssignmentRequest**对象的属性和关系。 |
| [列出 accessPackageAssignments](../api/accesspackageassignment-list.md) | [accessPackageAssignment](accesspackageassignment.md)集合 | 检索**accessPackageAssignment**对象的列表。 |
| [列出 accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)集合 | 检索**accessPackageAssignmentResourceRole**对象的列表。 |
| [获取 accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | 检索**accessPackageAssignmentResourceRole**对象。 |
| [列出 accessPackageCatalogs](../api/accesspackagecatalog-list.md) | [accessPackageCatalog](accesspackagecatalog.md)集合 | 检索**accessPackageCatalogs**对象的列表。 |
| [创建 accessPackageCatalog](../api/accesspackagecatalog-post.md) | [accessPackageCatalog](accesspackagecatalog.md) | 创建新的**accessPackageCatalog**对象。 |
| [获取 accessPackageCatalog](../api/accesspackagecatalog-get.md) | [accessPackageCatalog](accesspackagecatalog.md) | 读取**accessPackageCatalog**对象的属性和关系。 |
| [删除 accessPackageCatalog](../api/accesspackagecatalog-delete.md) | | 删除**accessPackageCatalog**。 |
| [列出 accessPackageCatalog 资源](../api/accesspackagecatalog-list-accesspackageresources.md) | [accessPackageResource](accesspackageresource.md)集合 | 检索**accessPackageResource**对象的列表。 |
| [列出 accessPackageCatalog 资源角色](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [accessPackageResourceRole](accesspackageresourcerole.md)集合 | 检索**accessPackageResourceRole**对象的列表。 |
| [列出 accessPackageResourceRequests](../api/accesspackageresourcerequest-list.md) | [accessPackageResourceRequest](accesspackageresourcerequest.md)集合 | 读取**accessPackageResourceRequest**对象的属性和关系。 |
| [创建 accessPackageResourceRequest](../api/accesspackageresourcerequest-post.md) | [accessPackageCatalog](accesspackageresourcerequest.md) | 创建新的**accessPackageResourceRequest**对象。 |

## <a name="see-also"></a>另请参阅

 - [什么是 Azure AD 权限管理？](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-overview)



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
