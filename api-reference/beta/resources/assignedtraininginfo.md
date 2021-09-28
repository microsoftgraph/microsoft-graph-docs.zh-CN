---
title: assignedTrainingInfo 资源类型
description: 表示攻击模拟和培训活动中的已分配培训信息。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 15caed31f7db60980e453e942653820dc8b348bc
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979564"
---
# <a name="assignedtraininginfo-resource-type"></a>assignedTrainingInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示攻击模拟和培训活动中的培训的作业信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignedUserCount|Int32|在攻击模拟和培训活动中分配了培训的用户数量。|
|completedUserCount|Int32|在攻击模拟和培训活动中完成培训的用户数量。|
|displayName|字符串|在攻击模拟和培训活动中显示培训名称。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignedTrainingInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignedTrainingInfo",
  "assignedUserCount": "Integer",
  "completedUserCount": "Integer",
  "displayName": "String"
}
```

