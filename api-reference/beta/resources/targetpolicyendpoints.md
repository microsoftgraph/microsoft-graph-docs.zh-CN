---
title: targetPolicyEndpoints 资源类型
description: 表示面向用户通知的平台。
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 9c1911900f4945d6f4b75d62c62457791fbb5c6a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939465"
---
# <a name="targetpolicyendpoints-resource-type"></a>targetPolicyEndpoints 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可定向到的平台，用于接收发送给用户的通知。  其中包括 Windows、iOS、Android 和 Web。 


## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|platformTypes|String collection|使用将通知分发筛选到特定平台或平台。 有效值为`Windows`、 `iOS` `Android`和。 `WebPush` 默认情况下，将启用所有推送终结点类型（Windows、iOS、Android 和 WebPush）。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetPolicyEndpoints",
  "baseType": null
}-->

```json
{
  "platformTypes": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetPolicyEndpoints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->