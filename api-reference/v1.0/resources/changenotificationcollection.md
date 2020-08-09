---
title: changeNotificationCollection 资源类型
description: 表示发送给订阅者的订阅通知的集合。
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 1eadd0fbc14fe9e6581ab6fa3375837653fc0859
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598505"
---
# <a name="changenotificationcollection-resource-type"></a>changeNotificationCollection 资源类型

命名空间：microsoft.graph

表示发送给订阅者的资源更改通知的集合。

有关详细信息，请参阅[使用 Microsoft GRAPH API 获取更改通知](webhooks.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
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
