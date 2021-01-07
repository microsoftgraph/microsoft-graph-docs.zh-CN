---
title: approvalStage 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性中审批设置的 approvalStages 属性。 指定每个阶段的主要、回退和升级审批者。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 158fae1675c26876daeb05b1571d7fd91855df72
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777699"
---
# <a name="approvalstage-complex-type"></a>approvalStage 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于访问包分配策略的 **requestApprovalSettings** 属性中审批设置的 **approvalStages** [属性](accesspackageassignmentpolicy.md)。 指定每个阶段的主要、回退和升级审批者。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | 请求在被自动拒绝之前可以等待响应的天数。 |
| isApproverJustificationRequired |布尔值 | 指示是否需要审批者提供批准请求的理由。 |
| isEscalationEnabled |布尔值 | 如果为 true，则在此审批阶段配置一个或多个升级审批者。 |
| escalationTimeInMinutes |Int32 | 如果需要升级，则请求可以挂起主要审批者的响应的时间。 |
| primaryApprovers | [userSet](userset.md) 集合| 将要求其批准请求的用户。 [singleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md)和[externalSponsors 的集合](externalsponsors.md)。 |
| escalationApprovers | [userSet](userset.md) 集合| 如果启用升级，并且主要审批者在升级时间之前未响应，则 escalationApprovers 是需要批准请求的用户。 它可以是 [singleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md) 和 [externalSponsors 的集合](externalsponsors.md)。|



## <a name="json-representation"></a>JSON 表示形式

以下是请求审批阶段的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalStage"
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


