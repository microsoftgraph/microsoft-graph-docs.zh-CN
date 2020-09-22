---
title: approvalStage 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性中的审批设置的 approvalStages 属性。 指定每个阶段的主、回退和升级审批者。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: df7e9ce4491ea7a887b79f79d354c9099ea9f5d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050141"
---
# <a name="approvalstage-complex-type"></a>approvalStage 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于[访问包分配策略](accesspackageassignmentpolicy.md)的**requestApprovalSettings**属性中的审批设置的**approvalStages**属性。 指定每个阶段的主、回退和升级审批者。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | 请求在被自动拒绝前可等待响应的天数。 |
| isApproverJustificationRequired |Boolean | 指示是否需要审批者提供审批请求的理由。 |
| isEscalationEnabled |Boolean | 如果为 true，则在此审批阶段中配置一个或多个升级审批者。 |
| escalationTimeInMinutes |Int32 | 如果需要升级，请求可以挂起主审批者的响应。 |
| primaryApprovers | [userSet](userset.md) 集合| 将要求用户批准请求的用户。 [SingleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md)和[externalSponsors](externalsponsors.md)的集合。 |
| escalationApprovers | [userSet](userset.md) 集合| 如果启用了升级，并且主审批者在升级时间之前没有响应，则 escalationApprovers 是将被要求批准请求的用户。 它可以是 [singleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md) 和 [externalSponsors](externalsponsors.md)的集合。|



## <a name="json-representation"></a>JSON 表示形式

以下是请求审批阶段的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalStage",
  "baseType": ""
}-->

```json

{
    "approvalStageTimeOutInDays": 14,
    "isApproverJustificationRequired": true,
    "isEscalationEnabled": true,
    "escalationTimeInMinutes": 11520,
    "primaryApprovers": [{"@odata.type": "microsoft.graph.userSet"}],
    "escalationApprovers": [{"@odata.type": "microsoft.graph.userSet"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "approvalSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


