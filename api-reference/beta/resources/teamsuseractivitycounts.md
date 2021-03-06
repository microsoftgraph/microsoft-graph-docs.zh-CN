---
title: teamsUserActivityCounts 资源类型
description: 表示按类型表示的活动枚举。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7e931d3488fce488710c638a0155ef0c5dd3a521
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766089"
---
# <a name="teamsuseractivitycounts-resource-type"></a>teamsUserActivityCounts 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示按类型表示的活动枚举。

## <a name="properties"></a>属性

| 属性            | 类型   | 说明                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| reportRefreshDate   | 日期   | 内容的最新日期。                              |
| reportDate          | 日期   | 用户执行活动的日期。        |
| teamChatMessages    | Int64  | 用户在团队聊天中发布的唯一消息数。 |
| privateChatMessages | Int64  | 用户在私人聊天中发布的唯一消息数。 |
| calls               | Int64  | 用户参与的唯一 1：1 呼叫数。   |
| 会议            | Int64  | 用户参与的唯一联机会议的数量。 |
| reportPeriod        | String | 报告涵盖的天数。                        |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```


