---
title: payloadTypes 资源类型
description: 表示原始或直观用户通知的数据内容，这些通知将传递到应用客户端接收此通知并由其使用。
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: a35d48839e6932274f4257ce475710ea904878c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521981"
---
# <a name="payloadtypes-resource-type"></a>payloadTypes 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此资源表示原始或直观用户通知的数据内容，这些通知将传递到应用客户端接收此通知并由其使用。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|rawContent|String|收到此通知的所有受支持的平台（Windows、iOS、Android 或 WebPush）上的应用程序客户端将传递给和使用的原始用户通知的通知内容。 RawContent 或 VisualContent 中至少有一个有效的 POST 通知请求。|
|visualContent|[visualProperties](visualproperties.md)|可视用户通知的可视内容，该通知将由每个受支持的平台（仅适用于 Windows、iOS 和 Android）上的通知平台使用，并为用户呈现。 RawContent 或 VisualContent 中至少有一个有效的 POST 通知请求。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.payloadTypes",
  "baseType": null
}-->

```json
{
  "rawContent": "String",
  "visualContent": {"@odata.type": "microsoft.graph.visualProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "payloadTypes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->