---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 6c67de6592d32c15e7d64112ce9ac31b6a5d4c41
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092424"
---
# <a name="office365groupsactivitycounts-resource-type"></a>office365GroupsActivityCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性               | 类型   | 说明                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | 日期   | 内容的最新日期。          |
| exchangeEmailsReceived | Int64  | 由组邮箱接收的电子邮件数。 |
| yammerMessagesPosted   | Int64  | 发布到 Yammer 组的邮件数。 |
| yammerMessagesRead     | Int64  | Yammer 组中读取的邮件数。 |
| yammerMessagesLiked    | Int64  | Yammer 组中的已赞邮件数。 |
| reportDate             | 日期   | 向组邮箱或邮件中发送了大量电子邮件的日期已在 Yammer 组中投递、读取或赞 |
| reportPeriod           | 字符串 | 报告覆盖的天数。    |

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


