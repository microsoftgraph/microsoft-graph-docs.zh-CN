---
title: monitoringRule 资源类型
description: 定义要监视的信号和阈值的规则，以及满足时要执行的操作。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 305db31c935329574a2b7d52403dc7664ff53f66
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067855"
---
# <a name="monitoringrule-resource-type"></a>monitoringRule 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义要监视的信号和阈值的规则，以及满足时要执行的操作。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|microsoft.graph.windowsUpdates.monitoringAction|    达到给定信号的阈值时触发的操作。 可取值为：`alertError`、`pauseDeployment`。|
|signal|microsoft.graph.windowsUpdates.monitoringSignal|要监视的信号。 可能的值是 `rollback` ：。|
|阈值|Int32|要触发操作的信号的阈值。 从 1 到 100 的整数 (包含) 。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
  "signal": "String",
  "threshold": "Integer",
  "action": "String"
}
```

