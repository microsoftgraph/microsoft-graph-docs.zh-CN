---
title: approvalSettings 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性。 提供其他设置，以选择必须批准每个请求的执行者。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e248e47cf94e2c26e80b505cbaead450e03561d4
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331387"
---
# <a name="approvalsettings-complex-type"></a>approvalSettings 复杂类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于`requestApprovalSettings` [访问包分配策略](accesspackageassignmentpolicy.md)的属性。 提供其他设置，以选择必须批准每个请求的执行者。 

## <a name="properties"></a>属性

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| isApprovalRequired | 布尔值 | 如果为 false，则此策略中的请求不需要审批。 |
| isApprovalRequiredForExtension | 布尔值| 如果为 false，则已有分配扩展其工作分配的用户不需要进行审批。 |
| isRequestorJustificationRequired | 布尔值 | 指示请求者是否需要提供其请求中的理由。 |
| approvalMode| String | 或`Serial`中`NoApproval` `SingleStage`的一个。 时`NoApproval` `isApprovalRequired`使用的是 false。 |
| approvalStages | [approvalStage](approvalstage.md)集合| 如果需要审批，则此集合的一个或两个元素将定义每个审批阶段。 如果不需要审批，则为空数组。  |

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
