---
title: commsNotifications 资源类型
description: 通信服务器用于在一个批处理中发送多个通知的通知列表。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4497e2e1ba28e7f2d0b203f8f982053c5eb8ae1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341443"
---
# <a name="commsnotifications-resource-type"></a>commsNotifications 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通信服务器用于在一个批处理中发送多个通知的通知列表。

## <a name="properties"></a>属性

| 属性       | 类型                                                 | 说明                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| 值          | [commsNotification](commsnotification.md)集合 | 资源中的更改通知。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
