---
title: attackSimulationRepeatOffender 资源类型
description: 表示攻击模拟和培训中重复的惯用用户。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: a78d474514a4975584425c18da71451dc0352e25
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979481"
---
# <a name="attacksimulationrepeatoffender-resource-type"></a>attackSimulationRepeatOffender 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户中已跨各种攻击模拟和培训计划多次获得攻击方式的用户。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|attackSimulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|攻击模拟和培训活动中的用户。|
|repeatOffenceCount|Int32|用户在攻击模拟和培训计划中的重复行为数量。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationRepeatOffender"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationRepeatOffender",
  "repeatOffenceCount": "Integer",
  "attackSimulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

