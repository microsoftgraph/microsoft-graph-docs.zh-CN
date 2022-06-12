---
title: operationError 资源类型
description: 描述 teamsAsyncOperation 中的错误。
ms.localizationpriority: medium
author: billbliss
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 0bdc08d7d98b4f926a1cd6a247ccb9b6d41b9d62
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034447"
---
# <a name="operationerror-resource-type"></a>operationError 资源类型

命名空间：microsoft.graph



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
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

