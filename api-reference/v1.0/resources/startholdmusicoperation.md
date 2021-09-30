---
title: startHoldMusicOperation 资源类型
description: 表示 startHoldMusic 操作的状态，通过调用 startHoldMusic API 触发。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1c38436cbb8fc7214663aaba9af450879dbd04f
ms.sourcegitcommit: cbad97d6a8ccb89b1822b30a11cc9b6f2670deda
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2021
ms.locfileid: "60016556"
---
# <a name="startholdmusicoperation-resource-type"></a>startHoldMusicOperation 资源类型

命名空间：microsoft.graph

表示 [startHoldMusic](../api/participant-startholdmusic.md) 操作的状态，通过调用 **startHoldMusic** API 触发。 继承自 [commsOperation](commsoperation.md)。

## <a name="properties"></a>属性

| 属性                       | 类型                        | 说明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | 字符串                      | 继承自 **commsOperation**。 唯一的客户端上下文字符串。 最多可包含 256 个字符。                                                                               |
| id                             | 字符串                      | 继承自 **commsOperation**。 服务器操作 ID。 只读。                                                                                            |
| resultInfo                     | [resultInfo](resultinfo.md) | 继承自 **commsOperation**。 结果信息。  只读。                                                                                            |
| status                         | 字符串                      | 继承自 **commsOperation**。 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。                                                 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.startHoldMusicOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```