---
title: addContentHeaderAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容标头的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 341af43f03d8a319c7aaec535681f21db0a7f7f4
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939101"
---
# <a name="addcontentheaderaction-resource-type"></a>addContentHeaderAction 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个操作，该操作指定要添加到信息中的内容标头的详细信息（如果适用）。

## <a name="properties"></a>属性

| 属性      | 类型   | 描述                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| alignment     | 字符串 | 可取值为：`left`、`right`、`center`。               |
| fontColor     | 字符串 | 标头使用的字体颜色。                      |
| fontName      | 字符串 | 要用于标头的字体的名称。                       |
| fontSize      | Int32  | 标头使用的字号。                              |
| 页脚        | Int32  | 文档顶部的页眉的边距。        |
| text          | 字符串 | 标头本身的内容。                            |
| uiElementName | 字符串 | 应在其中放置标头的 UI 元素的名称。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentHeaderAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "alignment": "String",
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "margin": 1024,
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->