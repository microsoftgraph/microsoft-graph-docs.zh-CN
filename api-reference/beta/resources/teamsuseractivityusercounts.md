---
title: teamsUserActivityUserCounts 资源类型
description: 表示按活动类型表示的每日用户数。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1ddb3e6e5e6a0b6fbb5c9973bec7e29f4492089
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766439"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>teamsUserActivityUserCounts 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示按活动类型表示的每日用户数。

## <a name="properties"></a>属性

| 属性            | 类型   | 说明                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| reportRefreshDate   | 日期   | 内容的最新日期。                              |
| reportDate          | 日期   | 用户执行活动的日期。        |
| teamChatMessages    | Int64  | 在团队聊天中发布消息的用户数量。       |
| privateChatMessages | Int64  | 在私人聊天中发布消息的用户数量。    |
| calls               | Int64  | 参与一对一呼叫的用户数。           |
| 会议            | Int64  | 参与联机会议的用户数。     |
| otherActions        | Int64  | 除报告中提供的公开操作类型外，处于活动状态但执行了其他活动的用户数 (发送或回复频道消息和聊天消息、安排或参与 1：1 呼叫和会议) 。 示例操作包括用户更改 Teams 状态或 Teams 状态消息或打开频道消息帖子但不回复的情况。 |
| reportPeriod        | String | 报告涵盖的天数。                        |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```


