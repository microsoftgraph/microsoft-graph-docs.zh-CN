---
title: printUsageByPrinter 资源类型
description: 描述指定时间段内打印机的打印活动 (usageDate) 。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: f41ee77c390f63d05b0b6076b21948f8bdad9d4cf3f8751be02a675db1fb967f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235336"
---
# <a name="printusagebyprinter-resource-type"></a>printUsageByPrinter 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

描述指定时间段内打印机的打印活动 (usageDate) 。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
| [列出 (每天) ](../api/reportroot-list-dailyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | 获取按打印机分组的每日打印使用情况摘要列表。 |
| [列出 (月) ](../api/reportroot-list-monthlyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | 获取按打印机分组的每月打印使用情况摘要列表。 |
| [Get](../api/printUsageByPrinter-get.md) | [printUsageByPrinter](printUsageByPrinter.md) | 读取 **printUsageByPrinter** 对象的属性和关系。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|此使用率摘要的 ID。|
|printerID|String|这些统计信息表示的打印机 ID。|
|usageDate|日期|与这些统计信息关联的日期。|
|completedBlackAndWhiteJobCount|Int64|打印机在关联日期完成的黑白打印作业数。|
|completedColorJobCount|Int64|打印机在关联日期完成的颜色打印作业数。|
|incompleteJobCount|Int64|在关联日期中已排入打印机队列但未完成的打印作业数。|

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

