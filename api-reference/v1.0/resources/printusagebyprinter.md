---
title: printUsageByPrinter 资源类型
description: 描述指定时间段内打印机的打印活动 (usageDate) 。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 8c5a69d01f0b8da05a5f72f5c2c7d9bacf10ff1a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517261"
---
# <a name="printusagebyprinter-resource-type"></a>printUsageByPrinter 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

描述指定时间段内打印机的打印活动 (usageDate) 。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [列出 (每天) ](../api/reportroot-list-dailyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | 获取按打印机分组的每日打印使用率摘要的列表。 |
| [列出 (每月) ](../api/reportroot-list-monthlyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | 获取按打印机分组的每月打印使用率摘要的列表。 |
| [获取](../api/printUsageByPrinter-get.md) | [printUsageByPrinter](printUsageByPrinter.md) | 读取 **printUsageByPrinter** 对象的属性和关系。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此使用率摘要的 ID。|
|printerID|String|由这些统计信息表示的打印机的 ID。|
|usageDate|日期|与这些统计信息关联的日期。|
|completedBlackAndWhiteJobCount|Int64|打印机在关联日期完成的黑白打印作业数。|
|completedColorJobCount|Int64|打印机在关联日期完成的颜色打印作业数。|
|incompleteJobCount|Int64|在关联日期排入打印机队列但未完成的打印作业数。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByPrinter",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByPrinter",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "printerId": "String"
}
```

