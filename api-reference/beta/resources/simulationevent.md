---
title: simulationEvent 资源类型
description: 表示攻击模拟和培训活动中的模拟事件。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5d0abb9606b549fb1349b1e98545dcf0f25e4fb7
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979530"
---
# <a name="simulationevent-resource-type"></a>simulationEvent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示攻击模拟和培训活动中的模拟事件。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|count|Int32|攻击模拟和培训活动中模拟事件的发生次数。|
|eventName|字符串|攻击模拟和培训活动中的模拟事件的名称。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationEvent",
  "eventName": "String",
  "count": "Integer"
}
```

