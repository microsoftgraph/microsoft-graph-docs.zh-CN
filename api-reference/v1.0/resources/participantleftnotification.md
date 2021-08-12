---
title: participantLeftNotification 资源类型
description: 包含有关已离开呼叫的基于策略的参与者的详细信息。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b0b74588d4014b53b79ec43adfd37443b52d60334319b8e126e1deccafb9dcd2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141390"
---
# <a name="participantleftnotification-resource-type"></a>participantLeftNotification 资源类型

命名空间：microsoft.graph

包含有关已离开呼叫的基于策略的参与者的详细信息。

在基于 [策略的](/microsoftteams/teams-recording-policy) 录制方案中，当由机器人呼叫管理的参与者离开会议时，会向机器人发送 ，以通知机器人有关参与者离开事件 `participantLeftNotification` 的详细信息。

## <a name="properties"></a>属性
| 属性       | 类型            | 说明                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| 通话           | [call](call.md) | 包含有关参与者加入事件的详细信息的 call 对象。 |
| participantId  | String          | 已离开会议的策略下的参与者的 ID。        |

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
