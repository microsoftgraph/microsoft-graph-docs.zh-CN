---
title: playPromptOperation 资源类型
description: 用于获取 playPrompt 操作的结果的 playPrompt 操作。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5adc385c5764371c1e2cab516bc33fd8504aecf5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447085"
---
# <a name="playpromptoperation-resource-type"></a>playPromptOperation 资源类型

命名空间： microsoft. graph

用于获取 playPrompt 操作的结果的 playPrompt 操作。

## <a name="properties"></a>属性

| 属性            | 类型                        | 说明|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| 适用       | String                      | 唯一的客户端上下文字符串。 最大限制为256个字符。                              |
| id                  | 字符串                      | 只读。                                                                         |
| resultInfo          | [resultInfo](resultinfo.md) | 结果信息。 只读。                                |
| status              | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。               |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
