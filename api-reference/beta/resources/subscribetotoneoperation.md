---
title: SubscribeToToneOperation 资源类型
description: 描述用于接收 DTMF 声音的订阅的创建响应格式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e35b3fe674c9f92b7dab723325d658facf13962f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520287"
---
# <a name="subscribetotoneoperation-resource-type"></a>SubscribeToToneOperation 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述用于接收 DTMF 声音的订阅的创建响应格式。

## <a name="properties"></a>属性

| 属性                       | 类型                        | 说明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| 适用                  | String                      | 客户端上下文。                                                                                                                               |
| id                             | String                      | 服务器操作 ID。 只读。                                                                                             |
| resultInfo                     | [resultInfo](resultinfo.md) | 结果信息。  只读。                                                                                             |
| status                         | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。                                                 |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscribeToToneOperation"
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
  "description": "subscribeToToneOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
