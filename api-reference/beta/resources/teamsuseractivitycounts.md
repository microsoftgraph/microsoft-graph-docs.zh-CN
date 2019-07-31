---
title: teamsUserActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9e1a40d962ded7825b72d31675cefb9869750866
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007618"
---
# <a name="teamsuseractivitycounts-resource-type"></a>teamsUserActivityCounts 资源类型

## <a name="properties"></a>属性

| 属性            | 类型   |
| :------------------ | :----- |
| reportRefreshDate   | 日期   |
| reportDate          | 日期   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| calls               | Int64  |
| 会议            | Int64  |
| reportPeriod        | String |


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
