---
title: teamsUserActivityUserDetail 资源类型
description: 以下是资源 JSON representaion。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 2e3f64c7065343712f6a9d9c6a114bf95f24c171
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823651"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>teamsUserActivityUserDetail 资源类型

## <a name="properties"></a>属性

| 属性                | 类型              |
| :---------------------- | :---------------- |
| reportRefreshDate       | 日期              |
| userPrincipalName       | 字符串            |
| lastActivityDate        | 日期              |
| 被               | 布尔           |
| deletedDate             | 日期              |
| assignedProducts        | String 集合 |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | 布尔           |
| reportPeriod            | String            |

## <a name="json-representation"></a>JSON 表示形式

以下是资源 JSON representaion。

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
