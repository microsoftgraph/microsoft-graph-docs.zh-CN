---
title: attackSimulationSimulationUserCoverage 资源类型
description: 表示攻击模拟和培训中用户的模拟覆盖范围。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 9caef11c29dbe003047d1013340c1fdae193d0d6
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979529"
---
# <a name="attacksimulationsimulationusercoverage-resource-type"></a>attackSimulationSimulationUserCoverage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示攻击模拟和培训中用户的累积模拟数据和结果。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|attackSimulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|攻击模拟和培训活动中的用户。|
|clickCount|Int32|用户在攻击模拟和培训计划中收到的有效负载中单击的链接数。|
|compromisedCount|Int32|用户在攻击模拟和培训计划中采取的攻击行动数量。|
|latestSimulationDateTime|DateTimeOffset|用户参与的最新攻击模拟和培训计划的日期和时间。|
|simulationCount|Int32|用户参与的攻击模拟和培训计划的数量。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationSimulationUserCoverage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationSimulationUserCoverage",
  "simulationCount": "Integer",
  "latestSimulationDateTime": "String (timestamp)",
  "clickCount": "Integer",
  "compromisedCount": "Integer",
  "attackSimulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

