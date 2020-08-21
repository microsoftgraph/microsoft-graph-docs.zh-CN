---
title: itemBody 资源类型
description: 表示项目正文的属性，例如邮件、事件或组帖子。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: grangeryy
ms.openlocfilehash: 2c224e4e9db87f8da98ef34296cc193eb2fb564c
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849756"
---
# <a name="itembody-resource-type"></a>itemBody 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示项目正文的属性，例如邮件、事件或组帖子。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|内容|String|项目的内容。|
|contentType|String|内容的类型。可能的值为 `text` 和 `html`。|

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
<!--
{
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
