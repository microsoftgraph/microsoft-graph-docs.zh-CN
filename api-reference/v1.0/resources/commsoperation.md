---
title: commsOperation 资源类型
description: 某个长时间运行的操作的状态。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5b7c6e8dcf68ad867f206c5702e7d7af9b48b470
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057064"
---
# <a name="commsoperation-resource-type"></a>commsOperation 资源类型

命名空间：microsoft.graph

表示某个长时间运行的操作的状态。

此资源可以作为对操作的响应返回，也可以作为 [commsNotification](commsNotification.md)的内容返回。  

如果作为操作的响应返回，则状态指示是否会出现后续通知。 例如，如果返回状态为或的操作 `completed` ，则 `failed` 不会通过通知通道进行任何后续操作。 

如果 `null` 操作或返回状态为或的操作 `notStarted` `running` ，后续更新将通过通知通道发出。

## <a name="properties"></a>属性

| 属性           | 类型                        | 说明                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| 适用      | String                      | 唯一的客户端上下文字符串。 最大限制为256个字符。                           |
| id                 | String                      | 操作 ID。 只读。                                                    |
| resultInfo         | [resultInfo](resultinfo.md) | 结果信息。 只读。                                              |
| 状态             | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。 |

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

