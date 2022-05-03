---
title: printOperationStatus 资源类型
description: 表示长时间运行的通用打印操作的当前状态。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 79cc94a38335bede616ef57bc33db12db63a5664
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176654"
---
# <a name="printoperationstatus-complex-type"></a>printOperationStatus 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示长时间运行的通用打印操作的当前状态。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|state|printOperationProcessingState|printOperation 的当前处理状态。 下表描述了有效值。 只读。|
|说明|String|printOperation 当前处理状态的人工可读说明。 只读。|

### <a name="printoperationprocessingstate-values"></a>printOperationProcessingState 值

|成员|值|Description|
|:---|:---|:---|
|notStarted|0|操作尚未启动。|
|运行|1|操作正在运行。|
|成功|2|操作已成功完成。|
|失败|3|操作失败。|
|unknownFutureValue|4|可变枚举 sentinel 值。 请勿使用。|

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

