---
title: teamsUserActivityUserDetail 资源类型
description: 下面是资源的 JSON representaion。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 73208044be5d3612303774f92dfced2302939de8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046354"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>teamsUserActivityUserDetail 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性                | 类型              |
| :---------------------- | :---------------- |
| reportRefreshDate       | 日期              |
| userPrincipalName       | String            |
| lastActivityDate        | 日期              |
| isDeleted               | Boolean           |
| deletedDate             | 日期              |
| assignedProducts        | String 集合 |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | Boolean           |
| reportPeriod            | String            |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON representaion。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```


