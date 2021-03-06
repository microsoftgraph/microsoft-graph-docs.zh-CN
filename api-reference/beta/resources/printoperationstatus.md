---
title: printOperationStatus 资源类型
description: 表示长时间运行的通用打印操作的当前状态。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 14c66cf59dc1715a16bd786657202a554d7c1753
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052549"
---
# <a name="printoperationstatus-complex-type"></a>printOperationStatus 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示长时间运行的通用打印操作的当前状态。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|state|printOperationProcessingState|PrintOperation 的当前处理状态。 有效值如下表所述。 只读。|
|说明|String|PrintOperation 的当前处理状态的可读说明。 只读。|

### <a name="printoperationprocessingstate-values"></a>printOperationProcessingState 值

|成员|值|说明|
|:---|:---|:---|
|notStarted|0|该操作尚未启动。|
|运行|1 |操作正在运行。|
|完成|2 |操作已成功完成。|
|未能|第三章|操作失败。|
|向 unknownfuturevalue|4 |Evolvable 枚举 sentinel 值。 请勿使用。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperationStatus"
}-->

```json
{
    "state": "String",
    "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

