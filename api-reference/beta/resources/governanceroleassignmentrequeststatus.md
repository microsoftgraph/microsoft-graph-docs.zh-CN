---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 表示 governanceRoleAssignmentRequest 的状态。
localization_priority: Normal
ms.openlocfilehash: 768ef092dbe52b0989277905bae03eee091ca8c6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340290"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>governanceRoleAssignmentRequestStatus 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的状态。


## <a name="properties"></a>属性
属性       | 类型 |说明|
|:----|:-------------|:-----|
|status |String| 角色分配请求的状态。 值可以是`InProgress`或`Closed`。|
|状态值 |String| 角色分配请求的子状态。 值可以是`Accepted`、 `PendingEvaluation`、 `Granted` `Denied` `PendingProvisioning` `Provisioned` `ProvisioningStarted`、、、、、、、、和。 `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `PendingRevocation` `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning`|
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
