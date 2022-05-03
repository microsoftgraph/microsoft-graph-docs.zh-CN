---
title: printTaskStatus 资源类型
description: 表示 printTask 的当前执行状态。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c484ef988e7452096d63fe103a6c45a8d22d06ff
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176334"
---
# <a name="printtaskstatus-resource-type"></a>printTaskStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [printTask](printtask.md) 的当前执行状态。 

>**注意：** 注册任务触发器的应用程序负责在处理完成时更新任务状态，除非相关打印作业已重定向到另一台打印机。

有关如何使用此资源向通用打印添加拉取打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|state|printTaskProcessingState|[printTask](printtask.md) 的当前处理状态。 下表描述了有效值。|
|说明|String|[printTask](printtask.md) 的当前处理状态的人工可读说明。|

### <a name="printtaskprocessingstate-values"></a>printTaskProcessingState 值

|成员|值|Description|
|:---|:---|:---|
|等待|0|任务执行处于挂起状态。|
|处理|1|任务执行正在进行中。|
|完成|2|任务执行已完成。|
|中止|3|任务执行已中止。|
|unknownFutureValue|4|可变枚举 sentinel 值。 请勿使用。|

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


