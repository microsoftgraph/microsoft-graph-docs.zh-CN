---
title: approvalStep 资源类型
description: 与 accessPackageAssignmentRequest 或 userConsentRequest 关联的 approvalStep 对象。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 510903f27dd751ac57b7df7dab0084f8ce89e35c
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651363"
---
# <a name="approvalstep-resource-type"></a>approvalStep 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD管理中](entitlementmanagement-overview.md)，与 关联的决策的 approvalStep 对象 `accessPackageAssignmentRequest` 。 它用于区分审批者可以处理审批工作流的不同步骤的决策。

在 [userConsentRequests](../resources/userconsentrequest.md)中，与请求关联的审批决策。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|[列出 approvalSteps](../api/approval-list-steps.md) | [approvalStep](approvalstep.md) 集合 | 列出 **与审批对象关联的 approvalStep** **对象。** |
|[获取审批步骤](../api/approvalstep-get.md) | [approvalStep](approvalstep.md) | 检索 **approvalStep 对象** 的属性。 |
|[更新 approvalStep](../api/approvalstep-update.md) | 无 | 对 approvalStep 对象应用 **批准或拒绝** 决定。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignedToMe|Boolean|指示是否将步骤分配给呼叫用户进行审阅。 只读。|
|displayName|String|策略创建者提供的标签，用于标识审批步骤。 只读。|
|id|String|与审批对象关联的步骤的标识符。 只读。|
|justification|String|与审批步骤决策相关联的理由。|
|reviewResult|String|此审批记录的结果。 可能的值包括 `NotReviewed` `Approved` `Denied` ：、、。|
|reviewedBy|[userIdentity](useridentity.md) 集合 | 审阅者的标识符。 只读。|
|reviewedDateTime|DateTimeOffset|记录决策的日期和时间。 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|状态|String|步骤状态。 可能的值 `InProgress` `Initializing` `Completed` ：、、、。 `Expired` 只读。|


## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|审批|[审批](../resources/approval.md) 集合|与 关联的决策的审批对象 `accessPackageAssignmentRequest` 。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStep",
}
-->
``` json
{
   "@odata.type":"#microsoft.graph.approvalStep",
   "id":"String (identifier)",
   "displayName":"String",
   "status":"String",
   "assignedToMe":true,
   "reviewedBy": [{"@odata.type": "microsoft.graph.userIdentity"}],
   "reviewedDateTime":"String (timestamp)",
   "reviewResult":"String",
   "justification":"String"
}
```
