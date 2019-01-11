---
title: onenoteOperationError 资源类型
description: 失败的 OneNote 操作中的错误
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: df0bfd768d26c751a303f42e1f1123b863388faa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837336"
---
# <a name="onenoteoperationerror-resource-type"></a>onenoteOperationError 资源类型

失败的 OneNote 操作中的错误

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|code|string|错误代码。|
|消息|string|错误消息。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
