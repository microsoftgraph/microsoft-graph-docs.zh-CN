---
title: addContentFooterAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容页脚的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 05bbd7ee4b2d4b2b9c4e772b19bd26c86d91cc69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508420"
---
# <a name="addcontentfooteraction-resource-type"></a>addContentFooterAction 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个操作，该操作指定要添加到信息中的内容页脚的详细信息（如果适用）。

## <a name="properties"></a>属性

| 属性      | 类型   | 说明                                                   |
| :------------ | :----- | :------------------------------------------------------------ |
| alignment     | String | 可取值为：`left`、`right`、`center`。               |
| fontColor     | String | 用于页脚的字体颜色。                      |
| fontName      | String | 要用于页脚的字体的名称。                       |
| fontSize      | Int32  | 用于页脚的字号。                              |
| 页脚        | Int32  | 文档底部的页眉的边距。     |
| text          | String | 页脚本身的内容。                            |
| uiElementName | String | 应在其中放置页脚的 UI 元素的名称。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addContentFooterAction",
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
  "description": "addContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->