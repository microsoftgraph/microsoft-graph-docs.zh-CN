---
title: simulationEventsContent 资源类型
description: 表示攻击模拟和培训活动中的模拟事件。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 0a35ce8a743a358ab319388dc9aa25fe88e32dec
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979534"
---
# <a name="simulationeventscontent-resource-type"></a>simulationEventsContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示攻击模拟和培训活动中的模拟事件。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|compromisedRate|双精度|在攻击模拟和培训活动中遭受模拟攻击的用户的实际百分比。|
|events|[simulationEvent](../resources/simulationevent.md) 集合|攻击模拟和培训活动中的模拟事件列表。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationEventsContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationEventsContent",
  "compromisedRate": "Double",
  "events": [
    {
      "@odata.type": "microsoft.graph.simulationEvent"
    }
  ]
}
```

