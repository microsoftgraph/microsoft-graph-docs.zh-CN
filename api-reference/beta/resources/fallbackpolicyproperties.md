---
title: fallbackPolicyProperties 资源类型
description: '允许在 iOS 终结点上为高优先级原始通知指定回退策略，其中包含用于指定回退等待时间（延迟）和相应的视觉通知内容的附加属性。 '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: a3ce59a23b5aec6dd43b370c3b67e9439b11937e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938960"
---
# <a name="fallbackpolicyproperties-resource-type"></a>fallbackPolicyProperties 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

允许在 iOS 终结点上为高优先级原始通知指定回退策略，其中包含用于指定回退等待时间（延迟）和相应的视觉通知内容的附加属性。 

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
| platformTypes | String collection | 指定开发人员想要对其启用原始 toast 通知回退的平台。 目前，如果指定了**fallbackPolicy** ，则**targetPolicy**必须包含`iOS`和可选的其他平台。 此外， **fallbackPolicy**是必需的，并且当前`iOS`仅支持 platformTypes 平台。 |
| fallbackDelayInSeconds | Int32 | 此延迟表示将直接 toast 通知发送到不提取原始通知的每个用户 iOS 设备订阅之前传递的时间量（以秒为单位）。 该值必须介于60和600之间。 |
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