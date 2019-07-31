---
title: teamsUserActivityUserDetail 资源类型
description: 下面是资源的 JSON representaion。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cbe6297388907f28f8841e0a1dcb2ec3ae788844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964352"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>teamsUserActivityUserDetail 资源类型

## <a name="properties"></a>属性

| 属性                | 类型              |
| :---------------------- | :---------------- |
| reportRefreshDate       | 日期              |
| userPrincipalName       | String            |
| lastActivityDate        | 日期              |
| isDeleted               | Boolean           |
| deletedDate             | 日期              |
| assignedProducts        | String collection |
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
