---
title: printTaskTrigger 资源类型
description: 根据关联的 printTaskDefinition 确定将执行新 printTask 的条件。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0a9ca4d06f43c9dd0964f0bb4c9614bfb4a78c1e
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091575"
---
# <a name="printtasktrigger-resource-type"></a>printTaskTrigger 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

确定根据关联的[printTaskDefinition](printtaskdefinition.md)触发新[printTask](printtask.md)时所依据的条件。

有关如何使用此资源将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持 pull 打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List](../api/printer-list-tasktriggers.md) | [printTaskTrigger](printtasktrigger.md)集合 | 获取与特定[打印机](printer.md)相关联的 printTaskTriggers 的列表。 |
| [获取](../api/printtasktrigger-get.md) | [printTaskTrigger](printtasktrigger.md) | 获取与特定[printTask](printtask.md)关联的 printTaskTrigger。 |


## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String|PrintTaskTrigger 的标识符。 只读。|
|event|printEvent|将导致触发新[printTask](printtask.md)的通用打印事件。 有效值如下表所述。|

### <a name="printevent-values"></a>printEvent 值

|成员|值|说明|
|:---|:---|:---|
|jobStarted|0|表示启动新的打印作业时发生的事件。|
|向 unknownfuturevalue|1 |Evolvable 枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|定义|[printTaskDefinition](printtaskdefinition.md)|将用于创建[printTask](printtask.md)的抽象定义（由 print 事件触发时）。 只读。|

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
