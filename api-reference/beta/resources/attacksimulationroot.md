---
title: attackSimulationRoot 资源类型
description: 为租户提供启动真实的网络钓鱼攻击并学习的功能。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e38107d7c6d95706508ea5260fa9e88c87774672
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519738"
---
# <a name="attacksimulationroot-resource-type"></a>attackSimulationRoot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为租户提供启动真实的网络钓鱼攻击并学习的功能。
这是一个抽象类型。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出模拟](../api/attacksimulationroot-list-simulations.md)|[模拟](../resources/simulation.md) 集合|从模拟导航属性获取模拟资源。|

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|simulations|[模拟](../resources/simulation.md) 集合|表示租户的攻击模拟和培训活动。|

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

