---
title: simulationReportOverview 资源类型
description: 表示攻击模拟和培训计划的概述报告。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5f096dbe931959707ad067ce3d11fcf0afac4bdb
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979566"
---
# <a name="simulationreportoverview-resource-type"></a>simulationReportOverview 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示攻击模拟和培训计划的概述。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|recommendedActions|[recommendedAction](../resources/recommendedaction.md) 集合|针对租户的建议操作列表，用于根据攻击模拟和培训活动攻击类型改进其安全状况。|
|resolvedTargetsCount|Int32|攻击模拟和培训活动中的有效用户数。|
|simulationEventsContent|[simulationEventsContent](../resources/simulationeventscontent.md)|攻击模拟和培训活动中的模拟事件摘要。|
|trainingEventsContent|[trainingEventsContent](../resources/trainingeventscontent.md)|攻击模拟和培训活动中的已分配培训摘要。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationReportOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationReportOverview",
  "resolvedTargetsCount": "Integer",
  "simulationEventsContent": {
    "@odata.type": "microsoft.graph.simulationEventsContent"
  },
  "trainingEventsContent": {
    "@odata.type": "microsoft.graph.trainingEventsContent"
  },
  "recommendedActions": [
    {
      "@odata.type": "microsoft.graph.recommendedAction"
    }
  ]
}
```

