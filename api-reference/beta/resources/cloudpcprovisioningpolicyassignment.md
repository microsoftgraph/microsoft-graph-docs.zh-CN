---
title: cloudPcProvisioningPolicyAssignment 资源类型
description: CloudPC 设置策略分配
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fbbdf76dfb184efdae7279b5d4970367995c0a6c
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378303"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a>cloudPcProvisioningPolicyAssignment 资源类型

命名空间：microsoft.graph

表示设置策略分配的已定义集合。


## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|设置策略分配的唯一标识符。 只读。 如果 `target` 是用户组，则 ID 显示为 {policyId} _ {groupId}。|
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
