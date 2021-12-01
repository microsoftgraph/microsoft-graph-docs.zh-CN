---
title: accessPackageAssignmentRequestRequirements 资源类型
description: 标识请求指定访问包所需的要求。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 96179dd106936d5f39d5636231788ad51837473e
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242317"
---
# <a name="accesspackageassignmentrequestrequirements-resource-type"></a>accessPackageAssignmentRequestRequirements 资源类型

命名空间：microsoft.graph

表示调用方必须满足的要求，才能成功为指定为 URL 一部分的 **accessPackage** 创建 **accessPackageAssignmentRequest。** 要求通过评估与 **accessPackage** 关联的策略来确定。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowCustomAssignmentSchedule|布尔值|指示是否允许请求者设置自定义计划。|
|isApprovalRequiredForAdd|布尔值|指示要添加的请求是否必须由审批者批准。|
|isApprovalRequiredForUpdate|布尔值|指示更新请求是否必须由审批者批准。|
|policyDescription|String|用户尝试使用请求访问的策略的说明。|
|policyDisplayName|String|用户显示名称请求访问权限的策略的一部分。|
|policyId|String|与这些要求关联的策略的标识符。 创建新分配请求时，可以使用此标识符。|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|强制执行计划限制（如果有）。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequestRequirements"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequestRequirements",
  "policyId": "String",
  "policyDisplayName": "String",
  "policyDescription": "String",
  "isApprovalRequiredForAdd": "Boolean",
  "isApprovalRequiredForUpdate": "Boolean",
  "allowCustomAssignmentSchedule": "Boolean",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```


