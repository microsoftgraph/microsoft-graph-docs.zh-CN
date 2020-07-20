---
title: printTaskStatus 资源类型
description: 表示 printTask 的当前执行状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c5d46cd0c8d14b6dc07873bc503d024928e2b2e3
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091577"
---
# <a name="printtaskstatus-resource-type"></a>printTaskStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[printTask](printtask.md)的当前执行状态。 

>**注意：** 注册任务触发器的应用程序负责在处理完成时更新任务状态，除非相关的打印作业已重定向到另一台打印机。

有关如何使用此资源将拉取打印支持添加到通用打印的详细信息，请参阅[扩展通用打印以支持 pull 打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|state|printTaskProcessingState|[PrintTask](printtask.md)的当前处理状态。 有效值如下表所述。|
|description|String|[PrintTask](printtask.md)的当前处理状态的可读说明。|

### <a name="printtaskprocessingstate-values"></a>printTaskProcessingState 值

|成员|值|说明|
|:---|:---|:---|
|决|0|任务执行挂起。|
|处理|1 |正在执行任务。|
|后|2 |任务执行已完成。|
|其间|3 |任务执行已中止。|
|向 unknownfuturevalue|4 |Evolvable 枚举 sentinel 值。 请勿使用。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printTaskStatus"
}-->

```json
{
  "state": {"@odata.type": "microsoft.graph.printTaskProcessingState"},
  "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printTaskStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
