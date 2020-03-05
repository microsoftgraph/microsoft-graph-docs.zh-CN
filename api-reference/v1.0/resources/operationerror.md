---
title: operationError 资源类型
description: 描述 teamsAsyncOperation 中的错误。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0cf550b0c15d5bd6632490d40eae04c0b4f5f3f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447281"
---
# <a name="operationerror-resource-type"></a>operationError 资源类型

命名空间： microsoft. graph



描述[teamsAsyncOperation](teamsasyncoperation.md)中的错误。

## <a name="operationerror-properties"></a>operationError 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|code|string (readonly)|操作错误代码。|
|message|string (readonly)|操作错误消息。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
