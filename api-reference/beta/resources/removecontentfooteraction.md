---
title: removeContentFooterAction 资源类型
description: 表示一个操作，该操作指定要从信息中删除的内容页脚的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76450b0d6b0f3a532a4e3472d2ce99ead8c933e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073444"
---
# <a name="removecontentfooteraction-resource-type"></a>removeContentFooterAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个操作，该操作指定要从信息中删除的内容页脚的详细信息（如果适用）。 如果由于更新或删除标签而要删除页脚， [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)或 [EvaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) api 可能会返回 **removeContentFooterAction** 。 该操作指示使用应用程序移除包含之前适用的内容页脚的特定 UI 元素。

## <a name="properties"></a>属性

| 属性       | 类型              | 说明                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| uiElementNames | String 集合 | 要删除的页脚的 UI 元素的名称。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentFooterAction",
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
  "description": "removeContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

