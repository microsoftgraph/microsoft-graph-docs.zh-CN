---
title: removeContentHeaderAction 资源类型
description: 表示一个操作，该操作指定要从信息中删除的内容标头的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 907113e20b5e4257a672190433efd055a628c17f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521150"
---
# <a name="removecontentheaderaction-resource-type"></a>removeContentHeaderAction 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个操作，该操作指定要从信息中删除的内容标头的详细信息（如果适用）。 如果由于更新或删除标签而要删除标头，则[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)或[EvaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) api 可能会返回**removeContentHeaderAction** 。 该操作指示使用应用程序移除包含之前适用的内容头的特定 UI 元素。

## <a name="properties"></a>属性

| 属性       | 类型              | 说明                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| uiElementNames | String 集合 | 要删除的标头的 UI 元素的名称。 |

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