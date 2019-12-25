---
title: playPromptOperation 资源类型
description: 用于获取 playPrompt 操作的结果的 playPrompt 操作。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ae7b1f33216d2d9ae9d867fca57fe2dd27e2e4df
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865771"
---
# <a name="playpromptoperation-resource-type"></a>playPromptOperation 资源类型

用于获取 playPrompt 操作的结果的 playPrompt 操作。

## <a name="properties"></a>属性

| 属性            | 类型                        | 说明|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| 适用       | String                      | 唯一的客户端上下文字符串。 最大限制为256个字符。                              |
| id                  | 字符串                      | 只读。                                                                         |
| resultInfo          | [resultInfo](resultinfo.md) | 结果信息。 只读。                                |
| 状态              | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。               |

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
