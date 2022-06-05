---
title: approvalSettings 复杂类型
description: 角色管理策略规则中定义的审批设置。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0fd8af9a314052dab87908fde5987850899e8f90
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900217"
---
# <a name="approvalsettings-complex-type"></a>approvalSettings 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

角色管理策略规则中定义的审批设置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|approvalMode|字符串|其中一`SingleStage``Serial`个 (`Parallel``NoApproval` 默认) 。 `NoApproval`是使用时间`isApprovalRequired`。`false`|
|approvalStages|[approvalStage](../resources/approvalstage.md) 集合|如果需要审批，则此集合的一个或两个元素定义审批的每个阶段。 如果不需要审批，则为空数组。|
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
      "@odata.type": "microsoft.graph.approvalStage"
    }
  ]
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


