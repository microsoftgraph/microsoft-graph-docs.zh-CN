---
title: monitoringRule 资源类型
description: 定义要监视的信号和阈值的规则，以及满足时要执行的操作。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3ae09d2f4a3badf62ffa22380372e597b7fd6a4f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792181"
---
# <a name="monitoringrule-resource-type"></a>monitoringRule 资源类型

命名空间：microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义要监视的信号和阈值的规则，以及满足时要执行的操作。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|microsoft.graph.windowsUpdates.monitoringAction|    达到给定信号的阈值时触发的操作。 可取值为：`alertError`、`pauseDeployment`、`unknownFutureValue`。|
|signal|microsoft.graph.windowsUpdates.monitoringSignal|要监视的信号。 可取值为：`rollback`、`unknownFutureValue`。|
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

