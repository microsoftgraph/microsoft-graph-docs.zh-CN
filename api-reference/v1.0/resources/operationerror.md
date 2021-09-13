---
title: operationError 资源类型
description: 描述 teamsAsyncOperation 中的错误。
ms.localizationpriority: medium
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b30a945dcbd19a6c1be0c276eec0b650b8251ea1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098508"
---
# <a name="operationerror-resource-type"></a>operationError 资源类型

命名空间：microsoft.graph



描述 [teamsAsyncOperation 中的错误](teamsasyncoperation.md)。

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

