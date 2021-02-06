---
title: approvalSettings 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性。 提供其他设置，以选择必须批准每个请求的人。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 99892e0943b993fe43edb4bd104fd2a3a8736a51
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135254"
---
# <a name="approvalsettings-complex-type"></a>approvalSettings 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于 `requestApprovalSettings` 访问包分配 [策略的属性](accesspackageassignmentpolicy.md)。 提供其他设置，以选择必须批准每个请求的人。 

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isApprovalRequired | Boolean | 如果为 false，则不需要批准此策略中的请求。 |
| isApprovalRequiredForExtension | Boolean| 如果为 false，则已拥有工作分配的用户不需要批准以扩展其工作分配。 |
| isRequestorJustificationRequired | Boolean | 指示请求者是否需要在请求中提供理由。 |
| approvalMode| 字符串 | 之 `NoApproval` 一， `SingleStage` 或 `Serial` 。 如果 `NoApproval` 为 `isApprovalRequired` false，则使用 。 |
| approvalStages | [approvalStage](approvalstage.md) 集合| 如果需要审批，则此集合的一个或两个元素定义审批的每个阶段。 如果不需要批准，则为空数组。  |

## <a name="json-representation"></a>JSON 表示形式

以下是请求审批设置属性的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings"
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


