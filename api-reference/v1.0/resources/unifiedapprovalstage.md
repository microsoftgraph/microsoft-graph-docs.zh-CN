---
title: unifiedApprovalStage 资源类型
description: 定义 unifiedRoleManagementPolicyApprovalRule 对象中审批阶段的设置。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b046071cb3468187d75ebd079b4329907e3550c5
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134055"
---
# <a name="unifiedapprovalstage-resource-type"></a>unifiedApprovalStage 资源类型

命名空间：microsoft.graph

定义 [unifiedRoleManagementPolicyApprovalRule](unifiedrolemanagementpolicyapprovalrule.md) 对象中审批阶段的设置。 指定每个阶段的主要审批者和升级审批者，以及是否需要审批和升级。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|approvalStageTimeOutInDays|Int32| 请求在自动被拒绝之前等待响应的天数。 |
|escalationApprovers|[subjectSet](../resources/subjectset.md) 集合| 当主要审批者不响应时，此阶段的升级审批者。|
|escalationTimeInMinutes|Int32|请求可以等待主要审批者的响应的时间，然后才能将其上报给升级审批者。|
|isApproverJustificationRequired|Boolean| 指示审批者是否必须为其响应提供理由。|
|isEscalationEnabled|Boolean| 指示是否已启用升级。|
|primaryApprovers|[subjectSet](../resources/subjectset.md) 集合| 此阶段的主要审批者。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unifiedApprovalStage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedApprovalStage",
  "approvalStageTimeOutInDays": "Integer",
  "isApproverJustificationRequired": "Boolean",
  "escalationTimeInMinutes": "Integer",
  "primaryApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "isEscalationEnabled": "Boolean",
  "escalationApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ]
}
```

