---
title: participantLeftNotification 资源类型
description: 包含有关已离开呼叫的基于策略的参与者的详细信息。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2730cd68e8d7ff6c5c238caeaee91fb4a821c836
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446634"
---
# <a name="participantleftnotification-resource-type"></a>participantLeftNotification 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关已离开呼叫的基于策略的参与者的详细信息。

在基于 [策略](/microsoftteams/teams-recording-policy) 的录制方案下，当机器人呼叫管理的参与者离开会议时，系统将会向机器人发送一个通知机器人，告知机器人有关参与者离开事件 `participantLeftNotification` 的详细信息。

## <a name="properties"></a>属性
| 属性       | 类型            | 说明                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| 通话           | [call](call.md) | 包含有关参与者加入事件的详细信息的调用对象。 |
| participantId  | String          | 策略下已离开会议的参与者的 ID。        |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantLeftNotification"
}-->
```json
{
  "participantId": "String",
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantLeftNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

