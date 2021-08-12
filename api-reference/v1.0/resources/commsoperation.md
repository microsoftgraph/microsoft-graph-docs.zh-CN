---
title: commsOperation 资源类型
description: 某些长时间运行的操作的状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dd924966c34d39ceb26e7b92077f01f085f9f6779896db439c1ae6c7a57eae9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130385"
---
# <a name="commsoperation-resource-type"></a>commsOperation 资源类型

命名空间：microsoft.graph

表示某些长时间运行的操作的状态。

此资源可返回为对操作的响应，或作为 [commsNotification 的内容返回](commsNotification.md)。  

当作为对操作的响应返回时，状态将指示是否将发生后续通知。 例如，如果返回状态为 或 的操作，将不会通过通知通道执行 `completed` `failed` 任何后续操作。 

如果操作或状态为 或 的操作返回，后续更新 `null` `notStarted` `running` 将通过通知通道提供。

## <a name="properties"></a>属性

| 属性           | 类型                        | 说明                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| clientContext      | String                      | 唯一的客户端上下文字符串。 最大限制为 256 个字符。                           |
| id                 | String                      | 操作 ID。 只读。                                                    |
| resultInfo         | [resultInfo](resultinfo.md) | 结果信息。 只读。                                              |
| status             | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。 |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

