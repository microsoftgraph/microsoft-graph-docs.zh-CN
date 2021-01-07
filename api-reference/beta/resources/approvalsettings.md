---
title: approvalSettings 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性。 提供其他设置，以选择必须批准每个请求的人。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 85d47e09de1b4d8f687a8dff2abf6aff1af0f21f
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777721"
---
# <a name="approvalsettings-complex-type"></a>approvalSettings 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于 `requestApprovalSettings` 访问包分配 [策略的属性](accesspackageassignmentpolicy.md)。 提供其他设置，以选择必须批准每个请求的人。 

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isApprovalRequired | 布尔值 | 如果为 false，则不需要批准此策略中的请求。 |
| isApprovalRequiredForExtension | 布尔值| 如果为 false，则已拥有工作分配的用户不需要批准来扩展其工作分配。 |
| isRequestorJustificationRequired | 布尔值 | 指示请求者是否需要在请求中提供理由。 |
| approvalMode| String | 之 `NoApproval` 一， `SingleStage` `Serial` 或 。 如果 `NoApproval` 为 `isApprovalRequired` false，则使用 。 |
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


