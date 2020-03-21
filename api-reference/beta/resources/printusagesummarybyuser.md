---
title: printUsageSummaryByUser 资源类型
description: 描述在指定时间段（usageDate）期间用户的打印活动。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 30769d9bd7ee76494b1582a3d7afc8a7f75bb07a
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895597"
---
# <a name="printusagesummarybyuser-resource-type"></a>printUsageSummaryByUser 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述在指定时间段（usageDate）期间用户的打印活动。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列表（每天）](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | 获取按用户分组的每日打印使用率摘要列表。 |
| [列表（每月）](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | 获取按月打印的使用情况摘要列表，按用户分组。 |
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