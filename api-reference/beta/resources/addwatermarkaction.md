---
title: addWatermarkAction 资源类型
description: 表示一个操作，该操作指定要添加到信息中的内容水印的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a94f517fe9f5da207febf9e776643a7c17c18d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508399"
---
# <a name="addwatermarkaction-resource-type"></a>addWatermarkAction 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个操作，该操作指定要添加到信息中的内容水印的详细信息（如果适用）。

## <a name="properties"></a>属性

| 属性      | 类型   | 说明                                                      |
| :------------ | :----- | :--------------------------------------------------------------- |
| fontColor     | String | 用于水印的字体颜色。                      |
| fontName      | String | 要用于水印的字体的名称。                       |
| fontSize      | Int32  | 用于水印的字号。                              |
| 布局        | String | 可取值为：`horizontal`、`diagonal`。                   |
| text          | String | 水印本身的内容。                            |
| uiElementName | String | 应在其中放置水印的 UI 元素的名称。 |

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