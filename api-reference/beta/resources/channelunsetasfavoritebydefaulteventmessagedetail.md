---
title: channelUnsetAsFavoriteByDefaultEventMessageDetail 资源类型
description: 表示有关默认情况下未设置为收藏的频道的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a30aecbd82d7b6a0ea7d6043cf1cfa832d40ae56
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535672"
---
# <a name="channelunsetasfavoritebydefaulteventmessagedetail-resource-type"></a>channelUnsetAsFavoriteByDefaultEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关未设置标志"isFavoriteByDefault"的通道的事件消息的详细信息。
如果频道的标记"isFavoriteByDefault"设置为 false，则频道不再对团队下频道列表中的所有团队成员可见。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|channelId|String|频道的唯一标识符。|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelUnsetAsFavoriteByDefaultEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelUnsetAsFavoriteByDefaultEventMessageDetail",
  "channelId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关默认情况下未设置为收藏的频道的事件消息的响应示例](/graph/system-messages/#channel-unset-as-favorite-by-default)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。