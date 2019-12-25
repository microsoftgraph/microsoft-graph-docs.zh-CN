---
title: unmuteParticipantOperation 资源类型
description: 描述呼叫参与者取消静音操作的响应格式。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3091caf53c4840db5c12ef856908b172a767624f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865756"
---
# <a name="unmuteparticipantoperation-resource-type"></a>unmuteParticipantOperation 资源类型

描述呼叫参与者取消静音操作的响应格式。

## <a name="properties"></a>属性

| 属性                       | 类型                        | 说明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| 适用                  | String                      | 唯一的客户端上下文字符串。 最多可以有256个字符。                                                                               |
| id                             | String                      | 服务器操作 ID。 只读。                                                                                            |
| resultInfo                     | [resultInfo](resultinfo.md) | 结果信息。  只读。                                                                                            |
| 状态                         | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。                                                 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unmuteParticipantOperation"
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
<!-- {
  "type": "#page.annotation",
  "description": "unmuteParticipantOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
