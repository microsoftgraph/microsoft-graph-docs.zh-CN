---
title: removeWatermarkAction 资源类型
description: 表示一个操作，该操作指定要从信息中删除的内容水印的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 271058e3ae56b2ded72c577f453d2af920d3ef0c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521136"
---
# <a name="removewatermarkaction-resource-type"></a>removeWatermarkAction 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个操作，该操作指定要从信息中删除的内容水印的详细信息（如果适用）。 如果由于更新或删除标签而要删除水印， [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)或[EvaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) api 可能会返回**removeWatermarkAction** 。 该操作指示使用应用程序移除包含之前适用的内容水印的特定 UI 元素。

## <a name="properties"></a>属性

| 属性       | 类型              | 说明                           |
| :------------- | :---------------- | :------------------------------------ |
| uiElementNames | String 集合 | 要删除的页脚的 UI 元素的名称。 |

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