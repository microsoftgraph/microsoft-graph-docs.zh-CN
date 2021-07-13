---
title: workloadActionDeploymentStatus 资源类型
description: 表示工作负荷操作部署状态。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a8c14b821ceabf8c8196a25c141ad8730f7151d6
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402089"
---
# <a name="workloadactiondeploymentstatus-resource-type"></a>workloadActionDeploymentStatus 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示工作负荷操作部署状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|actionId|String|工作负荷操作的唯一标识符。 必填。 只读。|
|deployedPolicyId|String|通过应用工作负荷操作创建的任何策略的标识符。 可选。 只读。|
|error|[microsoft.graph.genericError](../resources/genericerror.md)|部署工作负荷操作时发生的异常的详细信息。 可选。 必填。|
|lastDeploymentDateTime|DateTimeOffset|上次部署工作负荷操作日期和时间。 可选。|
|状态|workloadActionStatus|工作负荷操作部署的状态。 可取值为：`toAddress`、`completed`、`error`、`timeOut`、`inProgress`、`unknownFutureValue`。 必填。 只读。|

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
