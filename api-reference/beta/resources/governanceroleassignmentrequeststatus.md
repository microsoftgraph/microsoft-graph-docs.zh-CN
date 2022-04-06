---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 表示 governanceRoleAssignmentRequest 的状态。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: e023b40cd5c23c6b6f34d18c51eb7681354587b1
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723008"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>governanceRoleAssignmentRequestStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [governanceRoleAssignmentRequest 的状态](../resources/governanceroleassignmentrequest.md)。

## <a name="properties"></a>属性

| 属性      | 类型                                            | 说明                                                                                                                                                                                                                                                                                                                                                                                     |
| :------------ | :---------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 状态        | String                                          | 请求角色分配状态。 值可以是 或 `InProgress` `Closed`。                                                                                                                                                                                                                                                                                                           |
| subStatus     | String                                          | 请求的子角色分配状态。 值可以是 `Accepted``Granted``Denied``PendingEvaluation`、、、`PendingProvisioning`、`Provisioned`、、`PendingRevocation`、、 `AdminApproved``PendingAdminDecision``AdminDenied``TimedOut``Revoked``Failed``ProvisioningStarted``Canceled``PendingApprovalProvisioning``PendingApproval``FailedAsResourceIsLocked`和 。 |
| statusDetails | [keyValue](../resources/keyvalue.md) 集合 | 请求状态的详细信息角色分配请求。 它表示不同规则的评估结果。                                                                                                                                                                                                                                                                              |

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
