---
title: simulationReport 资源类型
description: 表示攻击模拟和培训活动的报告。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8f3e5991192d3d3f72e37e8ac5117a01d0138369
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979549"
---
# <a name="simulationreport-resource-type"></a>simulationReport 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示攻击模拟和培训活动的报告，包括活动概述和用户。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|概述|[simulationReportOverview](../resources/simulationreportoverview.md)|攻击模拟和培训计划概述。|
|simulationUsers|[userSimulationDetails](../resources/usersimulationdetails.md) 集合|表示租户用户在攻击模拟和培训活动中的联机操作。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.simulationReport"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationReport",
  "overview": {
    "@odata.type": "microsoft.graph.simulationReportOverview"
  },
  "simulationUsers": [
    {
      "@odata.type": "microsoft.graph.userSimulationDetails"
    }
  ]
}
```

