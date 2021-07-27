---
title: channelSetAsFavoriteByDefaultEventMessageDetail 资源类型
description: 表示有关默认情况下设置为收藏的频道的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35ddf629e82b55bb3ab475d65d6078e4607392a1
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535673"
---
# <a name="channelsetasfavoritebydefaulteventmessagedetail-resource-type"></a>channelSetAsFavoriteByDefaultEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关设置标志"isFavoriteByDefault"的通道的事件消息的详细信息。
如果某个频道的标记"isFavoriteByDefault"设置为 true，则频道对团队下频道列表中的所有团队成员可见。


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
  "@odata.type": "microsoft.graph.channelSetAsFavoriteByDefaultEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelSetAsFavoriteByDefaultEventMessageDetail",
  "channelId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关默认情况下设置为收藏的频道的事件消息的示例响应](/graph/system-messages/#channel-set-as-favorite-by-default)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。