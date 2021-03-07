---
title: printTaskTrigger 资源类型
description: 确定根据关联的 printTaskDefinition 执行新 printTask 的条件。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c0871f936b0935e6a599e79d6fb1a75f7e28f7ed
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517264"
---
# <a name="printtasktrigger-resource-type"></a>printTaskTrigger 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

确定根据关联的[printTaskDefinition](printtaskdefinition.md)触发新[printTask](printtask.md)的条件。

有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [List](../api/printer-list-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) 集合 | 获取与特定打印机相关联的 printTaskTriggers [列表](printer.md)。 |
| [获取](../api/printtasktrigger-get.md) | [printTaskTrigger](printtasktrigger.md) | 获取与特定 printTask 关联的[printTaskTrigger。](printtask.md) |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|printTaskTrigger 的标识符。 只读。|
|event|printEvent|将导致触发新 [printTask](printtask.md) 的通用打印事件。 下表介绍了有效值。|

### <a name="printevent-values"></a>printEvent 值

|成员|值|Description|
|:---|:---|:---|
|jobStarted|0|表示启动新打印作业时发生的事件。|
|unknownFutureValue|1 |可发展枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|definition|[printTaskDefinition](printtaskdefinition.md)|一个抽象定义，用于在打印事件触发时创建[printTask。](printtask.md) 只读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printTaskTrigger",
  "id": "String (identifier)",
  "event": "String"
}
```

