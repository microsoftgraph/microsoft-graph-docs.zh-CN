---
title: approvalStage 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性中审批设置的 approvalStages 属性。 指定每个阶段的主要、回退和升级审批者。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fd5a27a66d335dfe56acfbb0d30771ddbd9a703c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336380"
---
# <a name="approvalstage-complex-type"></a>approvalStage 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于访问包分配策略的 **requestApprovalSettings** 属性中审批设置的 **approvalStages** [属性](accesspackageassignmentpolicy.md)。 指定每个阶段的主要、回退和升级审批者。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | 请求在被自动拒绝之前可以等待响应的天数。 |
| isApproverJustificationRequired |Boolean | 指示是否需要审批者提供批准请求的理由。 |
| isEscalationEnabled |Boolean | 如果为 true，则在此审批阶段配置一个或多个上报审批者。 |
| escalationTimeInMinutes |Int32 | 如果需要升级，则请求可以挂起主要审批者的响应的时间。 |
| primaryApprovers | [userSet](userset.md) 集合| 将要求批准请求的用户。 [singleUser](singleuser.md)、[groupMembers](groupmembers.md)、[requestorManager](requestormanager.md)、[internalSponsors](internalsponsors.md) 和 [externalSponsors 的集合](externalsponsors.md)。 创建或更新策略 [时](accesspackageassignmentpolicy.md)，请在此集合中 **至少包含一个 userSet** 。 |
| escalationApprovers | [userSet](userset.md) 集合| 如果启用升级，并且主要审批者在升级时间之前未响应，则 escalationApprovers 是需要批准请求的用户。 它可以是 [singleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md) 和 [externalSponsors 的集合](externalsponsors.md)。  创建或更新策略时，[](accesspackageassignmentpolicy.md)如果阶段不需要升级审批者或不需要升级审批者，则此属性的值应为空集合。|



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


