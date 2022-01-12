---
title: workloadActionDeploymentStatus 资源类型
description: 表示工作负荷操作部署状态。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 763ad6e70969565f15f9db159a423d6ec1bbb4a2
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792041"
---
# <a name="workloadactiondeploymentstatus-resource-type"></a>workloadActionDeploymentStatus 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示工作负荷操作部署状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionId|String|工作负荷操作的唯一标识符。 必需。 只读。|
|deployedPolicyId|String|通过应用工作负荷操作创建的任何策略的标识符。 可选。 只读。|
|error|[microsoft.graph.genericError](../resources/genericerror.md)|部署工作负荷操作时发生的异常的详细信息。 可选。 必需。|
|lastDeploymentDateTime|DateTimeOffset|上次部署工作负荷操作日期和时间。 可选。|
|状态|workloadActionStatus|工作负荷操作部署的状态。 可取值为：`toAddress`、`completed`、`error`、`timeOut`、`inProgress`、`unknownFutureValue`。 必需。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadActionDeploymentStatus",
  "actionId": "String",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.genericError"
  },
  "deployedPolicyId": "String",
  "lastDeploymentDateTime": "String (timestamp)"
}
```
