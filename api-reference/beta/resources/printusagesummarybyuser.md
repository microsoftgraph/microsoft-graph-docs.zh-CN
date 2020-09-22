---
title: printUsageSummaryByUser 资源类型
description: 描述用户在指定时间段内的打印活动 (usageDate) 。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bba9f57799a36bef4a90b7c514a5be4b4846565e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070645"
---
# <a name="printusagesummarybyuser-resource-type"></a>printUsageSummaryByUser 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述用户在指定时间段内的打印活动 (usageDate) 。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 (每日) ](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | 获取按用户分组的每日打印使用率摘要列表。 |
| [每月 () 列表 ](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | 获取按月打印的使用情况摘要列表，按用户分组。 |
| [Get](../api/printusagesummarybyuser-get.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | 读取 printUsageSummaryByUser 对象的属性和关系。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|此使用率摘要的 ID。|
|userPrincipalName|String|由这些统计信息表示的用户的 UPN。|
|usageDate|日期|与这些统计信息关联的日期。|
|completedBlackAndWhiteJobCount|Int64|在关联日期代表用户完成的黑色和白色打印作业的数量。|
|completedColorJobCount|Int64|在关联日期代表用户完成的彩色打印作业的数量。|
|incompleteJobCount|Int64|在关联的日期上代表用户排队但未完成的打印作业数。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
}-->

```json
{
    "id": "String (identifier)",
    "userPrincipalName": "String (identifier)",
    "usageDate": "String (timestamp)",
    "completedBlackAndWhiteJobCount": 123456,
    "completedColorJobCount": 123456,
    "incompleteJobCount": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUsageSummaryByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

