---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 7e9f983d131d3b213689a48e10d8d23d3f99085b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968286"
---
# <a name="office365groupsactivitycounts-resource-type"></a>office365GroupsActivityCounts 资源类型

## <a name="properties"></a>属性

| 属性               | 类型   | 说明                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | 日期   | 内容最晚日期。          |
| exchangeEmailsReceived | Int64  | 通过组邮箱收到的电子邮件数。 |
| yammerMessagesPosted   | Int64  | 发布到 Yammer 组的消息数。 |
| yammerMessagesRead     | Int64  | Yammer 组中读取的消息数。 |
| yammerMessagesLiked    | Int64  | 喜欢 Yammer 组中的消息数。 |
| reportDate             | 日期   | 大量的电子邮件发送到组邮箱或日期已发布、 读取或喜欢 Yammer 组中的邮件数 |
| reportPeriod           | 字符串 | 报告涵盖天数。    |

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
