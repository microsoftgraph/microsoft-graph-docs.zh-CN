---
title: teamsUserActivityUserDetail 资源类型
description: 以下是资源 JSON representaion。
ms.openlocfilehash: 4e40ea4adf07450e6b51555df47579955a2a0286
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048143"
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
