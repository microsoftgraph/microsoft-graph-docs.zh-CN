---
title: 操作资源类型
description: 长时间运行的操作的状态。
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b1aabcf259d2d185d24b07e25b79d97e928ee245fd4f11acd848bc4f4a1ed646
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180584"
---
# <a name="operation-resource-type"></a>操作资源类型

命名空间：microsoft.graph

长时间运行的操作的状态。

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
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |操作开始时间。|
|lastActionDateTime| DateTimeOffset |操作的最后一个操作的时间。|
|status|operationStatus|操作的当前状态 `notStarted` ：、 `running` `completed``failed` |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

