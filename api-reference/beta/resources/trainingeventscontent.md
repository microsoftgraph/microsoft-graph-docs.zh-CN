---
title: trainingEventsContent 资源类型
description: 表示攻击模拟和培训活动中的培训计划。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 489e3b996f86a28f1d555489a30861e5251229f8
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979570"
---
# <a name="trainingeventscontent-resource-type"></a>trainingEventsContent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示攻击模拟和培训活动中的培训计划。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignedTrainingsInfos|[assignedTrainingInfo](../resources/assignedtraininginfo.md) 集合|在攻击模拟和培训活动中分配的培训及其信息的列表。|
|trainingsAssignedUserCount|Int32|在攻击模拟和培训活动中分配培训的用户数量。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.trainingEventsContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.trainingEventsContent",
  "trainingsAssignedUserCount": "Integer",
  "assignedTrainingsInfos": [
    {
      "@odata.type": "microsoft.graph.assignedTrainingInfo"
    }
  ]
}
```

