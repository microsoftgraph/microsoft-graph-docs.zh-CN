---
title: stopHoldMusicOperation 资源类型
description: 表示 stopHoldMusic 操作的状态，由对 stopHoldMusic API 的调用触发。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a0a30e783bfbcb08c613b2c0dd80a933d206830e
ms.sourcegitcommit: cbad97d6a8ccb89b1822b30a11cc9b6f2670deda
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2021
ms.locfileid: "60016553"
---
# <a name="stopholdmusicoperation-resource-type"></a>stopHoldMusicOperation 资源类型

命名空间：microsoft.graph

表示 [stopHoldMusic](../api/participant-stopholdmusic.md) 操作的状态，由对 **stopHoldMusic** API 的调用触发。 继承自 [commsOperation](commsoperation.md)。

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
  "@odata.type": "microsoft.graph.stopHoldMusicOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```