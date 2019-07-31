---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c1e441b142ef27abbdde4ac613ef8d75848f5001
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966550"
---
# <a name="office365groupsactivitycounts-resource-type"></a>office365GroupsActivityCounts 资源类型

## <a name="properties"></a>属性

| 属性               | 类型   | 说明                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | 日期   | 内容的最新日期。          |
| exchangeEmailsReceived | Int64  | 由组邮箱接收的电子邮件数。 |
| yammerMessagesPosted   | Int64  | 发布到 Yammer 组的邮件数。 |
| yammerMessagesRead     | Int64  | Yammer 组中读取的邮件数。 |
| yammerMessagesLiked    | Int64  | Yammer 组中的已赞邮件数。 |
| reportDate             | 日期   | 向组邮箱或邮件中发送了大量电子邮件的日期已在 Yammer 组中投递、读取或赞 |
| reportPeriod           | String | 报告覆盖的天数。    |

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
