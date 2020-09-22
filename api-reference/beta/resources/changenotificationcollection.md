---
title: changeNotificationCollection 资源类型
description: 表示发送给订阅者的订阅通知的集合。
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 4b273ecf2873842bb93b840241f2bf0a1741f1aa
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192174"
---
# <a name="changenotificationcollection-resource-type"></a>changeNotificationCollection 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示发送给订阅者的资源更改通知的集合。

有关详细信息，请参阅 [使用 Microsoft GRAPH API 获取更改通知](webhooks.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

| 属性 | 类型 | 描述 |
|:---------|:-----|:------------|
| validationTokens | collection(string) | 包含由 Microsoft Graph 生成的用于验证通知来源的应用程序生成的 JWT 令牌数组。 如果项目存在于值数组中，则 Microsoft Graph 将为每个不同的应用和租户对生成一个令牌。 请注意，通知可以包含使用同一通知 URL 订阅的各种应用和租户的项目组合。 仅为 [资源数据可选的更改通知](/graph/webhooks-with-resource-data.md) 提供。 |
| 值 |  ([changeNotification](changenotification.md)) 的集合 | 发送到通知 URL 的一组通知。 必填。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationCollection"
}-->

```json
{
  "value": [],
  "validationTokens": [
    "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
  ]
}
```

<!-- uuid: 8cc2599e-9740-4191-93fa-bc13c6f91564
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification collection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


