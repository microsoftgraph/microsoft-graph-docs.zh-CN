---
title: operationError 资源类型
description: 介绍 teamsAsyncOperation 中的错误。
ms.openlocfilehash: bcd8c989c4c69336165ef1ca29e1d114d524aa9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010607"
---
# <a name="operationerror-resource-type"></a>operationError 资源类型



介绍[teamsAsyncOperation](teamsasyncoperation.md)中的错误。

## <a name="operationerror-properties"></a>operationError 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|code|字符串 （只读）|操作错误代码。|
|message|字符串 （只读）|操作错误消息。|

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
