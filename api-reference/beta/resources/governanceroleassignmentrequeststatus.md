---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 表示 governanceRoleAssignmentRequest 的状态。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: e04b49fedf761ef3715d152fdc2a07a3af139bc3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695410"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>governanceRoleAssignmentRequestStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [governanceRoleAssignmentRequest 的状态](../resources/governanceroleassignmentrequest.md)。


## <a name="properties"></a>属性
属性       | 类型 |说明|
|:----|:-------------|:-----|
|status |String| 请求角色分配状态。 值可以是 `InProgress` 或 `Closed` 。|
|subStatus |String| 请求的子角色分配状态。 值可以是 `Accepted` `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `Provisioned` 、、、、、、、、 `PendingRevocation` `Revoked` `Canceled` `Failed` 和 `PendingApprovalProvisioning` `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `ProvisioningStarted` 。|
|statusDetails       |[keyValue](../resources/keyvalue.md) 集合| 请求角色分配的详细信息。 它表示不同规则的评估结果。 |

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


