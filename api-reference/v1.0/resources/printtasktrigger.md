---
title: printTaskTrigger 资源类型
description: 确定根据关联的 printTaskDefinition 执行新 printTask 的条件。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: b458b99c08a945198ddd1cd21678e0513a85a8b5
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944254"
---
# <a name="printtasktrigger-resource-type"></a>printTaskTrigger 资源类型

命名空间：microsoft.graph

确定根据关联的[printTaskDefinition](printtaskdefinition.md)触发新[printTask](printtask.md)的条件。

有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持下拉打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [List](../api/printer-list-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) 集合 | 获取与特定打印机相关联的 printTaskTriggers [列表](printer.md)。 |
| [获取](../api/printtasktrigger-get.md) | [printTaskTrigger](printtasktrigger.md) | 获取与特定[printTask 关联的 printTaskTrigger。](printtask.md) |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|printTaskTrigger 的标识符。 只读。|
|event|printEvent|将导致触发新 [printTask](printtask.md) 的通用 Print 事件。 下表介绍了有效值。|

### <a name="printevent-values"></a>printEvent 值

|成员|值|Description|
|:---|:---|:---|
|jobStarted|0|表示启动新打印作业时发生的事件。|
|unknownFutureValue|1|可发展枚举 sentinel 值。 请勿使用。|

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

