---
title: userSimulationDetails 资源类型
description: 表示租户的用户及其在攻击模拟和培训活动中的联机操作。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9ca7adee31eef9d197ac6ecba180be5fbaa7d697
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979550"
---
# <a name="usersimulationdetails-resource-type"></a>userSimulationDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户的用户以及用户在攻击模拟和培训活动中的联机操作。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignedTrainingsCount|Int32|在攻击模拟和培训活动中分配给用户的培训数量。|
|completedTrainingsCount|Int32|用户在攻击模拟和培训活动中完成的培训数量。|
|compromisedDateTime|DateTimeOffset|用户在攻击模拟和培训活动中遭到联机攻击的日期和时间。|
|inProgressTrainingsCount|Int32|用户在攻击模拟和培训活动中进行的培训数量。|
|isComprom一|布尔值|表示用户在攻击模拟和培训活动中是否受到威胁的标志。|
|reportedPhishDateTime|DateTimeOffset|用户在攻击模拟和培训活动中将有效负载报告为网络钓鱼的日期和时间。|
|simulationEvents|[userSimulationEventInfo](../resources/usersimulationeventinfo.md) 集合|攻击模拟和培训活动中的用户模拟事件列表。|
|simulationUser|[attackSimulationUser](../resources/attacksimulationuser.md)|攻击模拟和培训活动中的用户。|
|trainingEvents|[userTrainingEventInfo](../resources/usertrainingeventinfo.md) 集合|攻击模拟和培训活动中用户的培训事件列表。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userSimulationDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userSimulationDetails",
  "isCompromised": "Boolean",
  "compromisedDateTime": "String (timestamp)",
  "simulationEvents": [
    {
      "@odata.type": "microsoft.graph.userSimulationEventInfo"
    }
  ],
  "trainingEvents": [
    {
      "@odata.type": "microsoft.graph.userTrainingEventInfo"
    }
  ],
  "assignedTrainingsCount": "Integer",
  "completedTrainingsCount": "Integer",
  "inProgressTrainingsCount": "Integer",
  "reportedPhishDateTime": "String (timestamp)",
  "simulationUser": {
    "@odata.type": "microsoft.graph.attackSimulationUser"
  }
}
```

