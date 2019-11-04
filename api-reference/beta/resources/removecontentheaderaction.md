---
title: removeContentHeaderAction 资源类型
description: 表示一个操作，该操作指定要从信息中删除的内容标头的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 99f3b77607b34cb68cdef3fa9fc5658ed06b52ec
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938939"
---
# <a name="removecontentheaderaction-resource-type"></a>removeContentHeaderAction 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个操作，该操作指定要从信息中删除的内容标头的详细信息（如果适用）。 如果由于更新或删除标签而要删除标头，则[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)或[EvaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) api 可能会返回**removeContentHeaderAction** 。 该操作指示使用应用程序移除包含之前适用的内容头的特定 UI 元素。

## <a name="properties"></a>属性

| 属性       | 类型              | 描述                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| uiElementNames | String collection | 要删除的标头的 UI 元素的名称。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentHeaderAction",
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
  "description": "removeContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->