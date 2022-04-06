---
title: userTrainingEventInfo 资源类型
description: 表示在攻击模拟和培训活动中分配给用户的培训事件。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1a33cba93e61752d33b9829871b3280955895360
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758239"
---
# <a name="usertrainingeventinfo-resource-type"></a>userTrainingEventInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在攻击模拟和培训活动中分配给用户的培训事件。 培训课程包括分配培训、更新进行中的培训以及完成培训。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|培训的显示名称。|
|latestTrainingStatus|trainingStatus|分配给用户的培训的最新状态。 可取值为：`unknown`、`assigned`、`inProgress`、`completed`、`overdue`、`unknownFutureValue`。|
|trainingAssignedProperties|[userTrainingContentEventInfo](../resources/usertrainingcontenteventinfo.md)|分配给用户的培训的事件详细信息。|
|trainingCompletedProperties|[userTrainingContentEventInfo](../resources/usertrainingcontenteventinfo.md)|用户完成培训时的事件详细信息。|
|trainingUpdatedProperties|[userTrainingContentEventInfo](../resources/usertrainingcontenteventinfo.md)|用户更新/进行中的培训的事件详细信息。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userTrainingEventInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userTrainingEventInfo",
  "displayName": "String",
  "latestTrainingStatus": "String",
  "trainingAssignedProperties": {
    "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
  },
  "trainingUpdatedProperties": {
    "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
  },
  "trainingCompletedProperties": {
    "@odata.type": "microsoft.graph.userTrainingContentEventInfo"
  }
}
```

