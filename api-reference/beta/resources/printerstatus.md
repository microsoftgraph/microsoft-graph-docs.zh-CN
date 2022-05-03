---
title: printerStatus 资源类型
description: 表示打印机的处理状态，包括任何错误。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4b405fe00ab7dfe0e3ce90e79b1e7a82607f012c
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176542"
---
# <a name="printerstatus-resource-type"></a>printerStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示打印机的处理状态，包括任何错误。

## <a name="properties"></a>属性
| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|state|printerProcessingState|当前处理状态。 下表描述了有效值。 只读。|
|详细信息|printerProcessingStateDetail 集合|描述打印机处于当前状态的原因的详细信息列表。 下表描述了有效值。 只读。|
|说明|String|打印机当前处理状态的可读说明。 只读。|

### <a name="printerprocessingstate-values"></a>printerProcessingState 值

|成员|值|Description|
|:---|:---|:---|
|unknown|0|打印机报告的处理状态未知。|
|闲置|1|打印机处于空闲状态，可以接受新的打印作业。|
|处理|2|打印机目前正在处理打印作业，完成后将处理任何挂起的作业。|
|停止|3|打印机遇到问题 (例如，活动托盘) 中的纸张用完，在问题得到解决之前，无法继续当前的打印作业。 有关详细信息，请参阅 **详细信息** () 或 **说明** 值。|
|unknownFutureValue|4|可变枚举 sentinel 值。 请勿使用。|

### <a name="printerprocessingstatedetail-values"></a>printerProcessingStateDetail 值

[printerProcessingStateDetail 枚举类型](./printerprocessingstatedetail.md)

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerStatus"
}-->

```json
{
    "state": "String",
    "details": ["String"],
    "description": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

