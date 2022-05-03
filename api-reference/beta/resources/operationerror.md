---
title: operationError 资源类型
description: 描述 teamsAsyncOperation 中的错误。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: teamwork
author: billbliss
ms.openlocfilehash: 3634e55dca6328b40a9d21577183e8a5616c53f8
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176507"
---
# <a name="operationerror-resource-type"></a>operationError 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述 [teamsAsyncOperation](teamsasyncoperation.md) 中的错误。

## <a name="operationerror-properties"></a>operationError 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|code|string (readonly)|操作错误代码。|
|消息|string (readonly)|操作错误消息。|

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
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


