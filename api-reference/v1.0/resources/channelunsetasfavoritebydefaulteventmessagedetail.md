---
title: channelUnsetAsFavoriteByDefaultEventMessageDetail 资源类型
description: 表示有关默认情况下未设置为收藏的频道的事件消息的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4f9dab965db79fe08086af3327d727ac97713f3f
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322386"
---
# <a name="channelunsetasfavoritebydefaulteventmessagedetail-resource-type"></a>channelUnsetAsFavoriteByDefaultEventMessageDetail 资源类型

命名空间：microsoft.graph

表示有关未设置 [标志的通道](../resources/channel.md) `isFavoriteByDefault` 的事件消息的详细信息。

如果 **标志** 为 ，则频道不再对团队下 **频道列表中的所有** 团队成员 [](../resources/team.md) `isFavoriteByDefault` 可见 `false` 。

继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|channelId|String|频道的唯一 **标识符**。|
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
- [有关默认情况下未设置为收藏 **的频道的事件** 消息的响应示例](/graph/system-messages/#channel-unset-as-favorite-by-default)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。
