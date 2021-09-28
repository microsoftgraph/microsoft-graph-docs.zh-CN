---
title: attackSimulationTrainingUserCoverage 资源类型
description: 表示攻击模拟和培训中用户的培训覆盖范围。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: ac8772817fa4c5887a1ae84c80165794b4bed16c
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979558"
---
# <a name="attacksimulationtrainingusercoverage-resource-type"></a>attackSimulationTrainingUserCoverage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示攻击模拟和培训中用户的累积培训数据。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|attackSimulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|攻击模拟和培训活动中的用户。|
|userTrainings|[userTrainingStatusInfo](../resources/usertrainingstatusinfo.md) 集合|用户的已分配培训及其状态列表。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attackSimulationTrainingUserCoverage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attackSimulationTrainingUserCoverage",
  "userTrainings": [
    {
      "@odata.type": "microsoft.graph.userTrainingStatusInfo"
    }
  ],
  "attackSimulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

