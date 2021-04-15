---
title: printTaskTrigger 资源类型
description: 确定根据关联的 printTaskDefinition 执行新 printTask 的条件。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: de2da4f94894d9744fdfdd302b310251cd91fdb3
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766320"
---
# <a name="printtasktrigger-resource-type"></a>printTaskTrigger 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

确定根据关联的[printTaskDefinition](printtaskdefinition.md)触发新[printTask](printtask.md)的条件。

有关如何使用此资源向通用打印添加拉页打印支持的详细信息，请参阅扩展 [通用打印以支持下拉打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/printer-list-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md) 集合 | 获取与特定打印机相关联的 printTaskTriggers [列表](printer.md)。 |
| [Get](../api/printtasktrigger-get.md) | [printTaskTrigger](printtasktrigger.md) | 获取与特定打印机关联的特定 printTaskTrigger。 [](printer.md)|


## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|printTaskTrigger 的标识符。 只读。|
|event|printEvent|将导致触发新 [printTask](printtask.md) 的通用 Print 事件。 下表介绍了有效值。|

### <a name="printevent-values"></a>printEvent 值

|成员|值|说明|
|:---|:---|:---|
|jobStarted|0|表示启动新打印作业时发生的事件。|
|unknownFutureValue|1|可发展枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|definition|[printTaskDefinition](printtaskdefinition.md)|一个抽象定义，用于在打印事件触发时创建[printTask。](printtask.md) 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "event": {"@odata.type": "microsoft.graph.printEvent"},
  "definition": {"@odata.type": "microsoft.graph.printTaskDefinition"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


