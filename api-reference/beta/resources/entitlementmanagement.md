---
title: entitlementManagement 资源类型
description: 权利管理资源的容器。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c9c34a3699402f8d49fb2c0a0d9af3d5159a0eb3
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651711"
---
# <a name="entitlementmanagement-resource-type"></a>entitlementManagement 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

权利管理单一对象是权利管理资源的容器，包括[accessPackageCatalog、connectedOrganization](accesspackagecatalog.md)和[entitlementManagementSettings](entitlementmanagementsettings.md)。 [](connectedorganization.md)  有关资源的完整列表，请参阅 [权利管理概述](entitlementmanagement-overview.md)。

继承自 [实体](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|accessPackageAssignmentPolicies|[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 集合| 表示控制哪些主体可以通过访问包分配请求或分配访问包的策略。 |
|accessPackageAssignmentRequests|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|表示由用户或代表用户创建的访问包分配请求。|
|accessPackageAssignmentResourceRoles|[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) 集合| 表示主题通过访问包分配分配的资源特定角色。|
|accessPackageAssignments|[accessPackageAssignment](../resources/accesspackageassignment.md) 集合|表示向用户或组用户或 (主题授予) 。|
|accessPackageCatalogs|[accessPackageCatalog](../resources/accesspackagecatalog.md) 集合|表示一组访问包。|
|accessPackageResourceEnvironments|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 集合| 对资源所在的地理位置环境的引用。|
|accessPackageResourceRequests|[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) 集合|表示分别向目录添加或删除资源的请求。 |
|accessPackageResourceRoleScopes|[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) 集合| 对资源中的作用域和该范围的资源中的角色的引用。 |
|accessPackageResources|[accessPackageResource](../resources/accesspackageresource.md) 集合| 对与访问包目录关联的资源的引用。|
|accessPackages|[accessPackage](../resources/accesspackage.md) 集合|表示访问包对象。|
|connectedOrganizations|[connectedOrganization](../resources/connectedorganization.md) 集合|表示对其他组织（用户可以请求访问）的目录或域的引用。|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|表示控制权利管理Azure AD的设置。|

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

