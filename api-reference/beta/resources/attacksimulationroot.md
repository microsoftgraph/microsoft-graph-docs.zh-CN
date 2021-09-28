---
title: attackSimulationRoot 资源类型
description: 为租户提供启动真实的网络钓鱼攻击并学习的功能。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 56c0f8f8ce514e21b39e24494132ee6fec123d31
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979557"
---
# <a name="attacksimulationroot-resource-type"></a>attackSimulationRoot 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为租户提供启动真实的网络钓鱼攻击并学习的功能。
这是一个抽象类型。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出模拟](../api/attacksimulationroot-list-simulations.md)|[模拟](../resources/simulation.md) 集合|从模拟导航属性获取模拟资源。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|

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

