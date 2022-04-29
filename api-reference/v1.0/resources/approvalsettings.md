---
title: approvalSettings 资源类型
description: 角色管理策略规则中定义的审批设置。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2dc0240fd272e4d79209ee37bf79f293052eb400
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65134040"
---
# <a name="approvalsettings-resource-type"></a>approvalSettings 资源类型

命名空间：microsoft.graph

角色管理策略规则中定义的审批设置。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|approvalMode|String|其中一`SingleStage``Serial`个 (`Parallel``NoApproval` 默认) 。 `NoApproval`是使用时间`isApprovalRequired`。`false`|
|approvalStages|[unifiedApprovalStage](../resources/unifiedapprovalstage.md) 集合|如果需要审批，则此集合的一个或两个元素定义审批的每个阶段。 如果不需要审批，则为空数组。|
|isApprovalRequired|Boolean|指示是否需要批准此策略中的请求。|
|isApprovalRequiredForExtension|Boolean|指示用户是否需要批准才能扩展其分配。|
|isRequestorJustificationRequired|Boolean|指示请求者是否需要在其请求中提供理由。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.approvalSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approvalSettings",
  "isApprovalRequired": "Boolean",
  "isApprovalRequiredForExtension": "Boolean",
  "isRequestorJustificationRequired": "Boolean",
  "approvalMode": "String",
  "approvalStages": [
    {
      "@odata.type": "microsoft.graph.unifiedApprovalStage"
    }
  ]
}
```

