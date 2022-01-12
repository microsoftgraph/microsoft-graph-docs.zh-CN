---
title: managementActionDeploymentStatus 资源类型
description: 表示给定托管租户的部署状态。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2f9b8ce493239e4c33bc2f20c615897afab41d9b
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791880"
---
# <a name="managementactiondeploymentstatus-resource-type"></a>managementActionDeploymentStatus 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示给定托管租户的部署状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|managementActionId|String|管理操作标识符。 必需。 只读。|
|managementTemplateId|String|用于生成管理操作的管理模板标识符。 必需。 只读。|
|状态|managementActionStatus|管理操作的状态。 可取值为：`toAddress`、`completed`、`error`、`timeOut`、`inProgress`、`planned`、`resolvedBy3rdParty`、`resolvedThroughAlternateMitigation`、`riskAccepted`、`unknownFutureValue`。 必需。|
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
