---
title: participantJoiningNotification 资源类型
description: 包含有关加入呼叫的基于策略的参与者的详细信息。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e915697ba01e8968d7833e8701eaf1914984c28f
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430831"
---
# <a name="participantjoiningnotification-resource-type"></a>participantJoiningNotification 资源类型

命名空间：microsoft.graph

包含有关加入呼叫的基于策略的参与者的详细信息。

在基于 [策略](/microsoftteams/teams-recording-policy)的录制方案下，在策略下的参与者加入呼叫之前，会向与具有处理新参与者的可用容量的策略关联的自动程序 `participantJoiningNotification` 发送 。

响应 [负载中的 participantJoiningResponse](participantjoiningResponse.md) 应来自机器人。

## <a name="properties"></a>属性
| 属性       | 类型            | 说明                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| 通话           | [call](call.md) | 包含有关参与者加入事件的详细信息的 call 对象。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantJoiningNotification"
}-->
```json
{
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantJoiningNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
