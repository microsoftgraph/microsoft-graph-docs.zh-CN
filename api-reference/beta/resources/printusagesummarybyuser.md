---
title: printUsageSummaryByUser 资源类型
description: 描述指定时间段内用户的打印活动 (usageDate) 。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bba9f57799a36bef4a90b7c514a5be4b4846565e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753585"
---
# <a name="printusagesummarybyuser-resource-type"></a>printUsageSummaryByUser 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述指定时间段内用户的打印活动 (usageDate) 。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [列出 (每天) ](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | 获取每日打印使用情况摘要的列表，按用户分组。 |
| [列出 (月) ](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | 获取按用户分组的每月打印使用情况摘要列表。 |
| [获取](../api/printusagesummarybyuser-get.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | 读取 printUsageSummaryByUser 对象的属性和关系。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|此使用率摘要的 ID。|
|userPrincipalName|String|这些统计信息所代表的用户的 UPN。|
|usageDate|日期|与这些统计信息关联的日期。|
|completedBlackAndWhiteJobCount|Int64|在关联的日期代表用户完成的黑白打印作业数。|
|completedColorJobCount|Int64|在关联的日期代表用户完成的颜色打印作业数。|
|incompleteJobCount|Int64|代表用户（但不在关联日期）排队的打印作业数。|

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

