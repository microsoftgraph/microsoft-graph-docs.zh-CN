---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: eed42f5baf9a0130c69f9f8e6c026c9e0082d200
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115119"
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
| yammerMessages使用    | Int64  | 用户组中喜欢的邮件Yammer数。 |
| reportDate             | 日期   | 向组邮箱发送大量电子邮件的日期，或邮件在组组中发布、阅读或Yammer的日期 |
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


