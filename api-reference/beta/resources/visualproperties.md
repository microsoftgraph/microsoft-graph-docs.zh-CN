---
title: visualProperties 资源类型
description: '表示面向用户的视觉通知的可视内容（即标题和正文）。  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: f03563549cc1b2f42a274032dab7b310511c70c7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939178"
---
# <a name="visualproperties-resource-type"></a>visualProperties 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示面向用户的视觉通知的可视内容（即标题和正文）。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|title|String|可视用户通知的标题。 此字段对于 visual 通知负载来说是必需的。 |
|body|字符串|可视化用户通知的正文。 正文是可选的。|


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