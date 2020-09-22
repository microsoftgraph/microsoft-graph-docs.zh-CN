---
title: visualProperties 资源类型
description: '表示面向用户的视觉通知的可视内容（即标题和正文）。  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 62580847844a4b397ed117ea4b256cc4f035577a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057687"
---
# <a name="visualproperties-resource-type"></a>visualProperties 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示面向用户的视觉通知的可视内容（即标题和正文）。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|title|String|可视用户通知的标题。 此字段对于 visual 通知负载来说是必需的。 |
|body|String|可视化用户通知的正文。 正文是可选的。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.visualProperties",
  "baseType": null
}-->

```json
{
  "title": "String",
  "body": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

