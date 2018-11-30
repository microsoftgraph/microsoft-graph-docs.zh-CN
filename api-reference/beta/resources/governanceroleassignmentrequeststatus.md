---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 代表 governanceRoleAssignmentRequest 的状态。
ms.openlocfilehash: 06b0f17513d5d796d3fe71cbd3888963bc4a34ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043105"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>governanceRoleAssignmentRequestStatus 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的状态。


## <a name="properties"></a>属性
属性       | 类型 |说明|
|:----|:-------------|:-----|
|状态 |字符串| 角色分配请求的状态。 值可以是`InProgress`或`Closed`。|
|子状态 |字符串| Sub 角色分配请求的状态。 值可以是`Accepted`， `PendingEvaluation`， `Granted`， `Denied`， `PendingProvisioning`， `Provisioned`， `PendingRevocation`， `Revoked`， `Canceled`， `Failed`， `PendingApprovalProvisioning`， `PendingApproval`， `FailedAsResourceIsLocked`， `PendingAdminDecision`， `AdminApproved`， `AdminDenied`， `TimedOut`，和`ProvisioningStarted`。|
|statusDetails       |[keyValue](../resources/keyvalue.md)集合| 角色分配请求的状态的详细信息。 它所表示不同规则评估的结果。 |

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
  "statusDetails": [{"@odata.type": "microsoft.graph.keyvalue"}],
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->