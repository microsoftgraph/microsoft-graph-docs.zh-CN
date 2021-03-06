---
title: fallbackPolicy 资源类型
description: '仅允许为 iOS 终结点指定回退策略，并且该策略旨在用于高优先级原始通知。 '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 8d39f9b69eb4ebdfcab883adec10b70100efba4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071210"
---
# <a name="fallbackpolicy-resource-type"></a>fallbackPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

仅允许为 iOS 终结点指定回退策略，该策略旨在用于由于特定于平台的限制而无法发送到设备的高优先级原始通知 (例如，节电模式) 。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| endpointFallback | [fallbackpolicyProperties](fallbackpolicyproperties.md) | EndpointFallback 策略对象在终结点级别处理通知回退策略，目前限制为 iOS。 |   


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fallbackpolicy",
  "baseType": null
}-->

```json
{
  "endpointFallback": {"@odata.type": "microsoft.graph.fallbackpolicyProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fallbackpolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


