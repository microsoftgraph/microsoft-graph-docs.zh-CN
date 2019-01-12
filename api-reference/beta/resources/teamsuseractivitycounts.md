---
title: teamsUserActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987522"
---
# <a name="teamsuseractivitycounts-resource-type"></a>teamsUserActivityCounts 资源类型

## <a name="properties"></a>属性

| 属性            | 类型   |
| :------------------ | :----- |
| reportRefreshDate   | 日期   |
| reportDate          | 日期   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| 呼叫               | Int64  |
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
