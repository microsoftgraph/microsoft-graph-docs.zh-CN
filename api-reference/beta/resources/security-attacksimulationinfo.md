---
title: attackSimulationInfo 资源类型
description: 表示威胁提交攻击模拟信息
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d7caee88f2d097c344c9fdcb3ba64767893e0276
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856544"
---
# <a name="attacksimulationinfo-resource-type"></a>attackSimulationInfo 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示威胁提交的攻击模拟信息。 如果电子邮件是攻击模拟电子邮件，则电子邮件威胁提交将包含相应的攻击模拟信息。

## <a name="properties"></a>属性
| 属性              | 类型           | Description                          |
|:----------------------|:---------------|:-------------------------------------|
| attackSimDateTime     | DateTimeOffset | 指定攻击模拟的日期时间。   |
| attackSimDurationTime | 持续时间       | 指定攻击模拟的时间 () 持续时间  |
| attackSimId           | Guid           | 指定攻击模拟的活动 ID。 |
| attackSimUserId       | String         | 指定收到攻击模拟电子邮件的用户的用户 ID   |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.attackSimulationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.attackSimulationInfo",
  "attackSimId": "Guid",
  "attackSimDateTime": "String (timestamp)",
  "attackSimDurationTime": "String (duration)",
  "attackSimUserId": "String"
}
```

