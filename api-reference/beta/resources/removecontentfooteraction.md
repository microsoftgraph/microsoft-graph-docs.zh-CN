---
title: removeContentFooterAction 资源类型
description: 表示一个操作，指定要从信息中删除的内容页脚的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1e8de130b2ad346e8e1fee2077014eda9e9b94d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962071"
---
# <a name="removecontentfooteraction-resource-type"></a>removeContentFooterAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个操作，指定要从信息中删除的内容页脚的详细信息（如果适用）。 如果由于更新或删除标签而删除页脚，则 evaluateApplication、evaluateClassificationResults 或 [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) API 可能会返回 **removeContentFooterAction。** [](../api/informationprotectionlabel-evaluateApplication.md) [](../api/informationprotectionlabel-evaluateclassificationresults.md) 此操作指示使用应用程序删除包含以前适用的内容页脚的特定 UI 元素。

## <a name="properties"></a>属性

| 属性       | 类型              | 说明                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| uiElementNames | String collection | 要删除的页脚的 UI 元素的名称。 |

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

