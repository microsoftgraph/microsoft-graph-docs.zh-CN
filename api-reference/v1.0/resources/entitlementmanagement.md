---
title: entitlementManagement 资源类型
description: 权利管理资源的容器。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 85fb78ba5973e3493d2dd62b5e4685d0176dcbe7
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650907"
---
# <a name="entitlementmanagement-resource-type"></a>entitlementManagement 资源类型

权利管理单一对象是权利管理资源的容器，包括[accessPackageCatalog、connectedOrganization](accesspackagecatalog.md)和[entitlementManagementSettings](entitlementmanagementsettings.md)。 [](connectedorganization.md)  有关资源的完整列表，请参阅 [权利管理概述](entitlementmanagement-overview.md)。

继承自 [实体](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此值指示资源是单一的。 只读。 继承自 [实体](entity.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|accessPackages|[accessPackage](../resources/accesspackage.md) 集合|表示访问包对象。|
|assignmentRequests|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|表示由用户或代表用户创建的访问包分配请求。|
|assignments|[accessPackageAssignment](../resources/accesspackageassignment.md) 集合| 表示向用户或组用户或 (主题授予) 。|
|catalogs|[accessPackageCatalog](../resources/accesspackagecatalog.md) 集合| 表示一组访问包。|
|connectedOrganizations|[connectedOrganization](../resources/connectedorganization.md) 集合|表示对其他组织（用户可以请求访问）的目录或域的引用。|
|settings|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)| 表示控制权利管理Azure AD的设置。|

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


