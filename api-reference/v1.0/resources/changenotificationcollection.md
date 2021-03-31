---
title: changeNotificationCollection 资源类型
description: 表示发送给订阅者订阅通知的集合。
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 62098d3099549893165d60cb55699209e4034ccc
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469318"
---
# <a name="changenotificationcollection-resource-type"></a>changeNotificationCollection 资源类型

命名空间：microsoft.graph

表示发送到订阅者的资源更改通知的集合。

有关详细信息，请参阅 [Microsoft Graph API 通过更改通知](webhooks.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| validationTokens | collection(string) | 包含 Microsoft Graph 为应用程序生成的 JWT 令牌数组，用于验证通知的来源。 如果项目存在于值数组中，Microsoft Graph 将针对每个不同的应用和租户对生成一个令牌。 请记住，通知可以包含使用相同通知 URL 订阅的各种应用和租户的混合项目。 仅针对包含 [资源数据的更改通知提供可选](/graph/webhooks-with-resource-data.md) 。 |
| 值 | 集合 ([changeNotification](changenotification.md))  | 要发送到通知 URL 的通知集。 必填。 |

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

