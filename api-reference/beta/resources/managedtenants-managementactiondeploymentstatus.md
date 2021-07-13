---
title: managementActionDeploymentStatus 资源类型
description: 表示给定托管租户的部署状态。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: efd789a7b4b48098e8d679273da1152f6611a28c
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402308"
---
# <a name="managementactiondeploymentstatus-resource-type"></a>managementActionDeploymentStatus 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示给定托管租户的部署状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|managementActionId|String|管理操作标识符。 必填。 只读。|
|managementTemplateId|String|用于生成管理操作的管理模板标识符。 必填。 只读。|
|状态|managementActionStatus|管理操作的状态。 可取值为：`toAddress`、`completed`、`error`、`timeOut`、`inProgress`、`planned`、`resolvedBy3rdParty`、`resolvedThroughAlternateMitigation`、`riskAccepted`、`unknownFutureValue`。 必填。|
|workloadActionDeploymentStatuses|[microsoft.graph.managedTenants.workloadActionDeploymentStatus](../resources/managedtenants-workloadactiondeploymentstatus.md) 集合|给定管理操作工作负荷操作部署方案的集合。 可选。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionDeploymentStatus",
  "managementTemplateId": "String",
  "managementActionId": "String",
  "status": "String",
  "workloadActionDeploymentStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
    }
  ]
}
```
