---
title: channelAddedEventMessageDetail 资源类型
description: 表示有关添加到团队的频道的事件消息的详细信息。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 11fbca965d50069650b7be46325134ff397533e6
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535693"
---
# <a name="channeladdedeventmessagedetail-resource-type"></a>channelAddedEventMessageDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示有关添加到团队的频道的事件消息的详细信息。
将标准频道添加到团队时，将生成此消息。


继承自 [eventMessageDetail](../resources/eventmessagedetail.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|channelDisplayName|String|频道的显示名称。|
|channelId|String|频道的唯一标识符。|
|initiator|[identitySet](../resources/identityset.md)|事件的发起人。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelAddedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelAddedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>另请参阅
- [有关添加到团队的频道的事件消息的示例响应](/graph/system-messages/#channel-added)
- 有关其他类型的事件详细信息，请参阅 [系统消息](/graph/system-messages)。