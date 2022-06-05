---
title: approvalStage 复杂类型
description: 在权利管理中，用于访问包分配策略的 requestApprovalSettings 属性中审批设置的 approvalStages 属性。 指定每个阶段的主要、回退和升级审批者。 在 PIM 中，定义 unifiedRoleManagementPolicyApprovalRule 对象中审批阶段的设置。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cfaf9c314002e5fcc0dd2865216ea4346272e4b3
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900056"
---
# <a name="approvalstage-complex-type"></a>approvalStage 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在权利管理中，用于 [访问包分配策略](accesspackageassignmentpolicy.md)的 **requestApprovalSettings** 属性中审批设置的 **approvalStages** 属性。 指定每个阶段的主要、回退和升级审批者。

在 PIM 中，定义 [unifiedRoleManagementPolicyApprovalRule](unifiedrolemanagementpolicyapprovalrule.md) 对象中审批阶段的设置。 指定每个阶段的主要审批者和升级审批者，以及是否需要审批和升级。

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | 请求在自动被拒绝之前等待响应的天数。 |
| isApproverJustificationRequired |Boolean | 指示是否需要审批者提供批准请求的理由。 |
| isEscalationEnabled |Boolean | 如果为 true，则在此审批阶段配置一个或多个升级审批者。 |
| escalationTimeInMinutes |Int32 | 如果需要升级，则请求可以等待主要审批者的响应的时间。 |
| primaryApprovers | [userSet](userset.md) 集合| 将要求其批准请求的用户。 [singleUser](singleuser.md)、[groupMembers](groupmembers.md)、[requestorManager](requestormanager.md)、[internalSponsors](internalsponsors.md) 和 [externalSponsors 的](externalsponsors.md)集合。 创建或更新 [策略](accesspackageassignmentpolicy.md)时，此集合中至少包含一个 **userSet** 。 |
| escalationApprovers | [userSet](userset.md) 集合| 如果已启用升级，并且主要审批者未在升级时间之前做出响应，则升级者是将要求其批准请求的用户。 这可以是 [singleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md) 和 [externalSponsors 的](externalsponsors.md)集合。  创建或更新 [策略](accesspackageassignmentpolicy.md)时，如果没有升级审批者或阶段不需要升级审批者，则此属性的值应为空集合。|



## <a name="json-representation"></a>JSON 表示形式

下面是请求审批阶段的 JSON 表示形式。

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


