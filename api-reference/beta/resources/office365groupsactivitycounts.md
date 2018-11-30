---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 4f3a5bf02f5f477ebab036fc9afa5d35a8061138
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048262"
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
