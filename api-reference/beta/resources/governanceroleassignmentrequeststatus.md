---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 代表 governanceRoleAssignmentRequest 的状态。
localization_priority: Normal
ms.openlocfilehash: f4f0b23cf13de5beedb1964484ec4fbbb6e98720
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510174"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>governanceRoleAssignmentRequestStatus 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的状态。


## <a name="properties"></a>属性
属性       | 类型 |说明|
|:----|:-------------|:-----|
|状态 |String| 角色分配请求的状态。 值可以是`InProgress`或`Closed`。|
|子状态 |String| Sub 角色分配请求的状态。 值可以是`Accepted`， `PendingEvaluation`， `Granted`， `Denied`， `PendingProvisioning`， `Provisioned`， `PendingRevocation`， `Revoked`， `Canceled`， `Failed`， `PendingApprovalProvisioning`， `PendingApproval`， `FailedAsResourceIsLocked`， `PendingAdminDecision`， `AdminApproved`， `AdminDenied`， `TimedOut`，和`ProvisioningStarted`。|
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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequeststatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
