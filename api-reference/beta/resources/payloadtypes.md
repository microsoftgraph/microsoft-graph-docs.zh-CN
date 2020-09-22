---
title: payloadTypes 资源类型
description: 表示原始或直观用户通知的数据内容，这些通知将传递到应用客户端接收此通知并由其使用。
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 034770f2614bacdb9d160f4ff8d2efb4cd0a2c24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998094"
---
# <a name="payloadtypes-resource-type"></a>payloadTypes 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此资源表示原始或直观用户通知的数据内容，这些通知将传递到应用客户端接收此通知并由其使用。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|rawContent|String|将在所有受支持的平台上的应用程序客户端传递和使用的原始用户通知的通知内容 (Windows、iOS、Android 或 WebPush) 收到此通知。 RawContent 或 VisualContent 中至少有一个有效的 POST 通知请求。|
|visualContent|[visualProperties](visualproperties.md)|可视化用户通知的可视内容（将由每个受支持的平台上的通知平台使用） (Windows、iOS 和 Android 仅) 并为用户呈现。 RawContent 或 VisualContent 中至少有一个有效的 POST 通知请求。|


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

