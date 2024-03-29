---
title: changeNotificationCollection 资源类型
description: 表示发送给订阅者订阅通知的集合。
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 74af713c082cb8070b2329785647274c29c259bb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335393"
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
| validationTokens | collection(string) | 包含由 Microsoft Graph生成的 JWT 令牌数组，供应用程序验证通知的来源。 Microsoft Graph为项目的每个不同的应用和租户对生成一个令牌（如果它存在于值数组中）。 请记住，通知可以包含使用相同通知 URL 订阅的各种应用和租户的混合项目。 仅针对包含 [资源数据的更改通知提供可选](/graph/webhooks-with-resource-data.md) 。 |
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
``` json
{
  "@odata.type": "#microsoft.graph.changeNotificationCollection",
  "validationTokens": [
    "String"
  ],
  "value": [
    {
      "@odata.type": "microsoft.graph.changeNotification"
    }
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

