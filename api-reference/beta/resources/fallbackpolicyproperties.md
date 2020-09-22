---
title: fallbackPolicyProperties 资源类型
description: '允许在 iOS 终结点上为高优先级原始通知指定回退策略，使用其他属性指定回退等待时间 (延迟) 和相应的视觉通知内容。 '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: ee32b40f71c2540bb06b8b4478d0f896aac40b85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071206"
---
# <a name="fallbackpolicyproperties-resource-type"></a>fallbackPolicyProperties 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

允许在 iOS 终结点上为高优先级原始通知指定回退策略，使用其他属性指定回退等待时间 (延迟) 和相应的视觉通知内容。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| platformTypes | String 集合 | 指定开发人员想要对其启用原始 toast 通知回退的平台。 目前，如果指定了 **fallbackPolicy** ，则 **targetPolicy** 必须包含 `iOS` 和可选的其他平台。 此外，FallbackPolicy 是必需的，并且当前仅支持 **platformTypes** 平台 `iOS` 。 |
| fallbackDelayInSeconds | Int32 | 此延迟表示在将直接 toast 通知发送到不提取原始通知的每个用户 iOS 设备订阅之前，将 (以秒为单位的时间) 的时间量。 该值必须介于60和600之间。 |
| visualContent | [visualProperties](visualproperties.md)|在 iOS 上回退启动的原始到可视用户通知的可视内容。 |
 


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fallbackpolicyProperties",
  "baseType": null
}-->

```json
{
  "platformTypes": ["String"],
  "fallbackDelayInSeconds": 60,
  "visualContent": {"@odata.type": "microsoft.graph.visualProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fallbackpolicyProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

