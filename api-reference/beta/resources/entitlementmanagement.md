---
title: entitlementManagement 资源类型
description: 权利管理资源的容器。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2768db11986466e864884d611877cf93dab6ef1a
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694895"
---
# <a name="entitlementmanagement-resource-type"></a>entitlementManagement 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

权利管理单一实例是权利管理资源的容器，包括 [accessPackageCatalog](accesspackagecatalog.md)、 [connectedOrganization](connectedorganization.md) 和 [entitlementManagementSettings](entitlementmanagementsettings.md)。  有关资源的完整列表，请参阅 [权利管理概述](entitlementmanagement-overview.md)。

继承自 [entity](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

|关系|类型|描述|
|:---|:---|:---|
|accessPackageAssignmentPolicies|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 集合| 表示一个策略，该策略控制哪些受试者可以通过访问包分配请求或分配访问包。 |
|accessPackageAssignmentRequests|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|表示由用户或代表用户创建的访问包分配请求。|
|accessPackageAssignmentResourceRoles|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) 集合| 表示通过访问包分配为主题分配的特定于资源的角色。|
|accessPackageAssignments|[accessPackageAssignment](../resources/accesspackageassignment.md) 集合|将访问包分配给主题一段时间。|
|accessPackageCatalogs|[accessPackageCatalog](../resources/accesspackagecatalog.md) 集合|访问包的容器。|
|accessPackageResourceEnvironments|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 集合| 对资源所在的地理位置环境的引用。|
|accessPackageResourceRequests|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 集合|表示分别向目录添加或删除资源的请求。 |
|accessPackageResourceRoleScopes|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) 集合| 对资源中的作用域的引用，以及该范围的资源中的角色的引用。 |
|accessPackageResources|[accessPackageResource](../resources/accesspackageresource.md) 集合| 对与访问包目录关联的资源的引用。|
|accessPackages|[accessPackage](../resources/accesspackage.md) 集合|表示访问包对象。|
|connectedOrganizations|[connectedOrganization](../resources/connectedorganization.md) 集合|表示对用户可以请求访问权限的其他组织的目录或域的引用。|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|表示控制 Azure AD 权利管理行为的设置。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.entitlementManagement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagement",
  "id": "String (identifier)"
}
```

