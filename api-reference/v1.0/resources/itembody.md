---
title: itemBody 资源类型
description: 表示项目正文的属性，例如邮件、事件或组帖子。
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 44c48b916a625ce00a30474583fa45b2c1d37e3d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084305"
---
# <a name="itembody-resource-type"></a>itemBody 资源类型

命名空间：microsoft.graph

表示项目正文的属性，例如邮件、事件或组帖子。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|内容|String|项目的内容。|
|contentType|bodyType|内容的类型。可能的值为 `text` 和 `html`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

