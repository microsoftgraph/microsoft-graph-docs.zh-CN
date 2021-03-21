---
title: add的markAction 资源类型
description: 表示指定要添加到信息的内容水印的详细信息的操作（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: db493c57d6de7c840e5f0606743392698cb475b6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962124"
---
# <a name="addwatermarkaction-resource-type"></a>add的markAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示指定要添加到信息的内容水印的详细信息的操作（如果适用）。

## <a name="properties"></a>属性

| 属性      | 类型   | 说明                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| fontColor     | String | 用于水印的字体的颜色。                      |
| fontName      | String | 用于水印的字体的名称。                       |
| fontSize      | Int32  | 用于水印的字体大小。                              |
| layout        | String | 可取值为：`horizontal`、`diagonal`。                   |
| text          | String | 水印本身的内容。                            |
| uiElementName | String | 应放置水印的 UI 元素的名称。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addWatermarkAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "fontColor": "String",
  "fontName": "String",
  "fontSize": 1024,
  "layout": "String",
  "text": "String",
  "uiElementName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addWatermarkAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

