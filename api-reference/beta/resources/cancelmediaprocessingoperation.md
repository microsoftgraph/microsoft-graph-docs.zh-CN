---
title: CancelMediaProcessingOperation 资源类型
description: 此资源类型用于描述媒体处理取消操作的响应格式。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cc9142be9524b34ded7a2bd9315a6bb2cc1aa9ca
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006724"
---
# <a name="cancelmediaprocessingoperation-resource-type"></a>CancelMediaProcessingOperation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述媒体处理取消操作的响应格式。

## <a name="properties"></a>属性

| 属性                       | 类型                        | 说明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| 各种                            | 布尔                     | 指示是否停止所有操作或当前操作。                                                                                    |
| 适用                  | String                      | 客户端上下文。                                                                                                                               |
| id                             | String                      | 服务器操作 ID。 只读。                                                                                              |
| resultInfo                     | [resultInfo](resultinfo.md) | 结果信息。  只读。                                                                                              |
| 状态                         | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。                                                  |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation"
}-->
```json
{
  "all": true,
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
  "description": "cancelMediaProcessingOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
