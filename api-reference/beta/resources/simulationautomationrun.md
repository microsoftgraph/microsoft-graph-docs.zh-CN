---
title: simulationAutomationRun 资源类型
description: 表示租户上攻击模拟自动化的运行。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d5ca41d575ec90e150e8f0d54a37f0278b6b6bdb
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758312"
---
# <a name="simulationautomationrun-resource-type"></a>simulationAutomationRun 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户上攻击模拟自动化的运行。


## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出运行](../api/simulationautomation-list-runs.md)|[simulationAutomationRun](../resources/simulationautomationrun.md) 集合|获取攻击模拟自动化运行列表。|

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|endDateTime|DateTimeOffset|运行在攻击模拟自动化中的结束日期和时间。|
|id|String|攻击模拟自动化运行的唯一标识符。|
|simulationId|字符串|在攻击模拟自动化运行中启动的攻击模拟活动的唯一标识符。|
|startDateTime|DateTimeOffset|运行在攻击模拟自动化中开始的日期和时间。|
|状态|[simulationAutomationRunStatus](#simulationautomationrunstatus-values)|攻击模拟自动化运行的状态。 可能的值包括 `unknown`、`running`、`succeeded`、`failed`、`skipped`、`unknownFutureValue`。|

### <a name="simulationautomationrunstatus-values"></a>simulationAutomationRunStatus 值

|成员|说明 |
|:---|:---|
|unknown| 未定义模拟自动化运行的状态。 |
|running| 模拟自动化运行正在运行。 |
|succeeded| 已成功运行模拟自动化。 |
|failed| 模拟自动化运行失败。 |
|已跳过| 已跳过模拟自动化的运行。 |
|unknownFutureValue| 可发展枚举 sentinel 值。 请勿使用。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.simulationAutomationRun",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationAutomationRun",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "simulationId": "String",
  "startDateTime": "String (timestamp)",
  "status": "String"
}
```

