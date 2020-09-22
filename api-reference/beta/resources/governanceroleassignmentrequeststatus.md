---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 表示 governanceRoleAssignmentRequest 的状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 9b0af5326bb9c819ded03ab9497e155cb0dab7c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081684"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>governanceRoleAssignmentRequestStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的状态。


## <a name="properties"></a>属性
属性       | 类型 |说明|
|:----|:-------------|:-----|
|状态 |字符串| 角色分配请求的状态。 值可以是 `InProgress` 或 `Closed` 。|
|状态值 |字符串| 角色分配请求的子状态。 值可以是、、、、、、、、、、 `Accepted` `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `Provisioned` `PendingRevocation` `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning` `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` 和 `ProvisioningStarted` 。|
|statusDetails       |[keyValue](../resources/keyvalue.md) 集合| 角色分配请求状态的详细信息。 它表示不同规则的评估结果。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


