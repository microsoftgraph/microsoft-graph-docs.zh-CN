---
title: entitlementManagement 资源类型
description: 包含权利管理资源的单一方法。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: db9b09efeea88ee3fc1d1dcfefab8d1ddb1c789e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242285"
---
# <a name="entitlementmanagement-resource-type"></a>entitlementManagement 资源类型

权利管理单一对象是权利管理资源的容器，包括[accessPackageCatalog、connectedOrganization](accesspackagecatalog.md)和[entitlementManagementSettings](entitlementmanagementsettings.md)。 [](connectedorganization.md)  有关资源的完整列表，请参阅 [权利管理概述](entitlementmanagement-root.md)。

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
|accessPackages|[accessPackage](../resources/accesspackage.md) 集合|访问包。|
|assignmentRequests|[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 集合|访问包分配请求。|
|assignments|[accessPackageAssignment](../resources/accesspackageassignment.md) 集合|访问程序包分配。|
|catalogs|[accessPackageCatalog](../resources/accesspackagecatalog.md) 集合|访问包目录。|
|connectedOrganizations|[connectedOrganization](../resources/connectedorganization.md) 集合|已连接的组织。|
|设置|[entitlementManagementSettings](../resources/entitlementmanagementsettings.md)|权利管理设置。|

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


