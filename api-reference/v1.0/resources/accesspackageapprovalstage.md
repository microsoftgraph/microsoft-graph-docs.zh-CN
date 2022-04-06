---
title: accessPackageApprovalStage 资源类型
description: 用于审批设置的 stages 属性。 指定每个阶段的主要、回退和升级审批者。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cffd48048af6d9b44ef475cdc3adcc6d9f0da05f
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608294"
---
# <a name="accesspackageapprovalstage-complex-type"></a>accessPackageApprovalStage 复杂类型

命名空间：microsoft.graph

用于访问包分配策略 [中审批设置的](accesspackageassignmentapprovalsettings.md) **stages** [属性](accesspackageassignmentpolicy.md)。 指定每个阶段的主要、回退和升级审批者。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|durationBeforeAutomaticDenial|期限|请求在被自动拒绝之前可以等待响应的天数。|
|durationBeforeEscalation|期限|如果需要升级，则请求可以挂起主要审批者的响应的时间。|
|escalationApprovers|[subjectSet](../resources/subjectset.md) 集合|如果启用升级，并且主要审批者在升级时间之前未响应，则 escalationApprovers 是需要批准请求的用户。 |
|fallbackEscalationApprovers|[subjectSet](../resources/subjectset.md) 集合|作为回退升级审批者的主体（通常是用户）。|
|fallbackPrimaryApprovers|[subjectSet](../resources/subjectset.md) 集合|作为回退主要审批者的主体（通常是用户）。|
|isApproverJustificationRequired|Boolean|指示是否需要审批者提供批准请求的理由。|
|isEscalationEnabled|布尔|如果 `true`为 ，则在此审批阶段配置一个或多个 **escalationApprovers** 。|
|primaryApprovers|[subjectSet](../resources/subjectset.md) 集合|将要求审批请求的主体（通常是用户）。 [singleUser](singleuser.md)、[groupMembers](groupmembers.md)、[requestorManager](requestormanager.md)、[internalSponsors 或](internalsponsors.md) [externalSponsors 的集合](externalsponsors.md)。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageApprovalStage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageApprovalStage",
  "durationBeforeAutomaticDenial": "String (duration)",
  "isApproverJustificationRequired": "Boolean",
  "isEscalationEnabled": "Boolean",
  "durationBeforeEscalation": "String (duration)",
  "primaryApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "fallbackPrimaryApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "escalationApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "fallbackEscalationApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ]
}
```


