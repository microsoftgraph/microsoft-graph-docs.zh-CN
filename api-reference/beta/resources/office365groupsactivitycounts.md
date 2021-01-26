---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: a212028e4ba9d38ea38e99c835d89fe1fe7d850b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980694"
---
# <a name="office365groupsactivitycounts-resource-type"></a>office365GroupsActivityCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性               | 类型   | 说明                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | 日期   | 内容的最新日期。          |
| exchangeEmailsReceived | Int64  | 组邮箱接收的电子邮件数。 |
| yammerMessagesPosted   | Int64  | 张贴到 Yammer 组的消息数。 |
| yammerMessagesRead     | Int64  | Yammer 组中读取的消息数。 |
| yammerMessages在    | Int64  | Yammer 组中喜欢的消息数。 |
| reportDate             | 日期   | 向组邮箱发送大量电子邮件或 Yammer 组中发布、阅读或喜欢大量邮件的日期 |
| reportPeriod           | String | 报告涵盖的天数。    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeEmailsReceived": 1024, 
  "yammerMessagesPosted": 1024, 
  "yammerMessagesRead": 1024, 
  "yammerMessagesLiked": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


