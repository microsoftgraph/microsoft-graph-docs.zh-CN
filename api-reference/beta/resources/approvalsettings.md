---
title: approvalSettings 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性。 提供其他设置，以选择必须批准每个请求的执行者。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a3c674b6bb21ddebfbb63f60d1ec2d2b62077f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050144"
---
# <a name="approvalsettings-complex-type"></a>approvalSettings 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于 `requestApprovalSettings` [访问包分配策略](accesspackageassignmentpolicy.md)的属性。 提供其他设置，以选择必须批准每个请求的执行者。 

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isApprovalRequired | Boolean | 如果为 false，则此策略中的请求不需要审批。 |
| isApprovalRequiredForExtension | Boolean| 如果为 false，则已有分配扩展其工作分配的用户不需要进行审批。 |
| isRequestorJustificationRequired | Boolean | 指示请求者是否需要提供其请求中的理由。 |
| approvalMode| String | `NoApproval`或中的 `SingleStage` 一个 `Serial` 。 `NoApproval`时使用的是 `isApprovalRequired` false。 |
| approvalStages | [approvalStage](approvalstage.md) 集合| 如果需要审批，则此集合的一个或两个元素将定义每个审批阶段。 如果不需要审批，则为空数组。  |

## <a name="json-representation"></a>JSON 表示形式

以下是请求审批设置属性的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings",
  "baseType": ""
}-->

```json
{
    "isApprovalRequired": true,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": true,
    "approvalMode": "Serial",
    "approvalStages": [{"@odata.type": "microsoft.graph.approvalStage"}]
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


