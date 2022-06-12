---
title: 操作资源类型
description: 长时间运行的操作的状态。
ms.localizationpriority: medium
author: billbliss
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: e43d86c5c53ce95855bdb0ccd42c3a43049073ca
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034528"
---
# <a name="operation-resource-type"></a>操作资源类型

命名空间：microsoft.graph

长时间运行的操作的状态。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |操作的开始时间。|
|lastActionDateTime| DateTimeOffset |操作的最后一个操作的时间。|
|status|operationStatus|操作的当前状态： `notStarted`， ， `running``completed``failed` |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

