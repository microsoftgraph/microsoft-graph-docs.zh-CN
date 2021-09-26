---
title: cloudPcProvisioningPolicyAssignment 资源类型
description: CloudPC 预配策略分配
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: fba54fda5ad20142909b7fea7c01bb117e5b3911
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767389"
---
# <a name="cloudpcprovisioningpolicyassignment-resource-type"></a>cloudPcProvisioningPolicyAssignment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示已定义的设置策略分配集合。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|预配策略分配的唯一标识符。 只读。 如果 `target` 为用户组，则 ID 显示为 {policyId} \_ {groupId}。|
|target|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|预配策略的分配目标。 目前，此策略支持的唯一目标为用户组。 有关详细信息，请参阅 [cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md)。 |

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
