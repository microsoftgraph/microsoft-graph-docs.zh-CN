---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 28ac5ad72a9e0b7e32336b397c0df114abf6fc9b88368f983dd84413ca4fe96e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226138"
---
# <a name="office365groupsactivitycounts-resource-type"></a>office365GroupsActivityCounts 资源类型

命名空间：microsoft.graph

## <a name="properties"></a>属性

| 属性               | 类型   | 说明                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | 日期   | 内容的最新日期。          |
| exchangeEmailsReceived | Int64  | 组邮箱接收的电子邮件数。 |
| yammerMessagesPosted   | Int64  | 发送到组的邮件Yammer数量。 |
| yammerMessagesRead     | Int64  | 在邮件组中读取Yammer数。 |
| yammerMessages使用    | Int64  | 在用户组中喜欢的邮件Yammer数量。 |
| reportDate             | 日期   | 向组邮箱发送大量电子邮件的日期，或在组组中发布、阅读或点Yammer的日期 |
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


