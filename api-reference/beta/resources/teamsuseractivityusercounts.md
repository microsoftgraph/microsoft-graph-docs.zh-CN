---
title: teamsUserActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
ms.openlocfilehash: f4e10f1e34d4c6bdbed83279b98632c504630bc7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330455"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>teamsUserActivityUserCounts 资源类型

## <a name="properties"></a>属性

| 属性            | 类型   |
| :------------------ | :----- |
| reportRefreshDate   | 日期   |
| reportDate          | 日期   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| 呼叫               | Int64  |
| 会议            | Int64  |
| otherActions        | Int64  |
| reportPeriod        | String |

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
