---
title: remove使用markAction 资源类型
description: 表示一个操作，指定要从信息中删除的内容水印的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2a2365b2c9bc1080db9b6bf58b2035d88832881a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960353"
---
# <a name="removewatermarkaction-resource-type"></a>remove使用markAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个操作，指定要从信息中删除的内容水印的详细信息（如果适用）。 如果由于更新或删除标签而删除水印，则 evaluateApplication、evaluateClassificationResults 或 [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) API 可能会返回 [](../api/informationprotectionlabel-evaluateapplication.md)[](../api/informationprotectionlabel-evaluateclassificationresults.md)**removeIngmarkAction。** 此操作指示使用应用程序删除包含以前适用的内容水印的特定 UI 元素。

## <a name="properties"></a>属性

| 属性       | 类型              | 说明                           |
| :------------- | :---------------- | :------------------------------------ |
| uiElementNames | String collection | 要删除的页脚的 UI 元素的名称。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeWatermarkAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "uiElementNames": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeWatermarkAction resource",
  "keywords": "",  
  "section": "documentation",
  "tocPath": ""
}-->

