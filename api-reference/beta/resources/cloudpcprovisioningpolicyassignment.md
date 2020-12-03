---
title: cloudPcProvisioningPolicyAssignment 资源类型
description: CloudPC 设置策略分配
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 06a90efc67b483fed569a4e7029a74dac4f7f9ee
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563700"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a>cloudPcProvisioningPolicyAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示设置策略分配的已定义集合。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|设置策略分配的唯一标识符。 只读。 如果 `target` 是用户组，则 ID 显示为 {policyId} _ {groupId}。|
|target|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|预配策略的分配目标。 目前，此策略支持的唯一目标是用户组。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
    "groupId": "String"
  }
}
```
