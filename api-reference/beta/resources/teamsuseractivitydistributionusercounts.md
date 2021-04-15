---
title: teamsUserActivityDistributionUserCounts 资源类型
description: 表示选定时段内按活动类型表示的用户数。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3d4fa8b3aec98a03d7e51819db0dc4797367f499
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766921"
---
# <a name="teamsuseractivitydistributionusercounts-resource-type"></a>teamsUserActivityDistributionUserCounts 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示选定时段内按活动类型表示的用户数。

## <a name="properties"></a>属性

| 属性            | 类型   | 说明                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| reportRefreshDate   | 日期   | 内容的最新日期。                              |
| teamChatMessages    | Int64  | 用户在团队聊天中发布的唯一消息数。 |
| privateChatMessages | Int64  | 用户在私人聊天中发布的唯一消息数。 |
| calls               | Int64  | 用户参与的唯一 1：1 呼叫数。   |
| 会议            | Int64  | 用户参与的唯一联机会议的数量。 |
| reportPeriod        | String | 报告涵盖的天数。                        |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```


