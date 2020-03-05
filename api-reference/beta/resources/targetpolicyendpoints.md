---
title: targetPolicyEndpoints 资源类型
description: 表示面向用户通知的平台。
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 92ff6d0748e24fd58154f596188f25c51bdc6403
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520000"
---
# <a name="targetpolicyendpoints-resource-type"></a>targetPolicyEndpoints 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可定向到的平台，用于接收发送给用户的通知。  其中包括 Windows、iOS、Android 和 Web。 


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|platformTypes|String 集合|使用将通知分发筛选到特定平台或平台。 有效值为`Windows`、 `iOS` `Android`和。 `WebPush` 默认情况下，将启用所有推送终结点类型（Windows、iOS、Android 和 WebPush）。 |

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