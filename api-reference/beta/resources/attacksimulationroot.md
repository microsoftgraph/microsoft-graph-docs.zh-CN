---
title: attackSimulationRoot 资源类型
description: 提供启动组织可以从中学习的真实的网络钓鱼攻击的能力。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: b83d13c6541b036bf3096f6ba6e99a9f4dfb79f5
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757652"
---
# <a name="attacksimulationroot-resource-type"></a>attackSimulationRoot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供启动组织可以从中学习的真实的网络钓鱼攻击的能力。
这是一个抽象类型。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出模拟](../api/attacksimulationroot-list-simulations.md)|[模拟](../resources/simulation.md) 集合|获取租户的攻击模拟培训计划列表。|
|[列出 simulationAutomations](../api/attacksimulationroot-list-simulationautomations.md)|[simulationAutomation](../resources/simulationautomation.md) 集合|获取租户的攻击模拟自动化列表。|

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|simulations|[模拟](../resources/simulation.md) 集合|表示租户中的攻击模拟培训活动。|
|simulationAutomations|[simulationAutomation](../resources/simulationautomation.md) 集合|表示为在租户上运行而创建的模拟自动化。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attackSimulationRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationRoot"
}
```

